# Adventure Works - Executive Summary

![Executive Summary](https://github.com/user-attachments/assets/c380daa1-1a3e-4829-9667-efcb83c3a8b7)


### Dashboard Link : https://docs.google.com/spreadsheets/d/13hSVy2znulV3emNhgHvvnjhGjZfgYUFU/edit?usp=drive_link&ouid=115038762084746239933&rtpof=true&sd=true

## Problem Statement

You've just received an email marked "URGENT" from the executives at Adventure Works. 
They've heard about your expertise in data analytics and have a pressing request: "We need 
a comprehensive Power BI report ASAP!" Now, the room you find yourself in isn't just any 
room; you're in the executive suite of Adventure Works, surrounded by the company's top 
minds. These decision-makers juggle multi-million-dollar budgets, eyeing global expansion 
and continually adapting to ever-changing market dynamics. They don't just want data; they 
need actionable insights, and they need them now. 

The executives understand that in the modern business landscape, data isn't just an asset; it's 
the essence of strategic decision-making. Asyou look around, you see various department 
heads clutching different pieces of the data puzzle—sales printouts, customer 
demographics, and inventory reports—but they're fragmented, disjointed, and not speaking 
to each other. The executives look to you to make the data understandable and actionable. 
You've been given a significant responsibility: to harness the potential of sales and customer 
data that will influence high-stakes decision-making. So, are you ready to dive in?

More specifically, you were asked to:

- Create a variety of visualizations, including a table, column chart, line chart, and Key Performance Indicators (KPIs), to represent complex sales and customer data in a digestible format.

- Customize these visuals by setting specific colors and adding tooltips, enhancing the user experience and accessibility of the data.

- Implement forecasting functionalities on the line chart, empowering the executives to anticipate future sales trends and take proactive measures.

- Integrate a Q&A visual into the report, enabling the executive team to query the data directly and receive timely insights.



### Steps followed 

* Step 1 : Download and open the Power BI report titled "Adventure Works Executive Summary.pbix" from this link:
        https://drive.google.com/file/d/12ar9Cxf6Aj69t0RSt8wqjGd6NHjahb4g/view?usp=drive_link
* Step 2 : Add the first visual:

        1. Start by going to the blank canvas and locate the Visualizations pane on the right hand side
           of your screen. Select the Table icon (it appears as a small grid) to create an empty table 
           visualization on the canvas.
        2. Find the Data pane on the right-hand side of the screen. Locate your Sales and Customers tables 
           there. Select the Sales table to expand it and view its fields.
        3. Drag Product ID from the Data pane to the Columns well in the Visualizationspane. Then drag 
           Product Name, Order ID, Order Status, and Order Total into the same Columns well.
        4. To format this table visual and change its appearance, select the Format tab. Expand the Style 
           presets option and select the Minimal preset from the available dropdown.
        5. You will notice that your table is a bit small or not well-positioned. Select the edges of the 
           table visualization box on your canvas to resize it and place the visualization on the right side 
           of the canvas.

* Step 3 : Add the second visual:

        1. Select the white space of your canvas to deselect the table visualization. Then, select the 
           Clustered Column chart icon in the Visualizations pane. An empty column chart will appear on 
           the canvas.
        2. Drag Product Category from the Sales table and drop it into the X-Axis well.
        3. Now, drag Order Total from the same Sales table and drop it into the Y-Axis well.
        4. To format this column chart and change its appearance, select the Format tab. In the Format tab, 
           locate the Columns > Colors option. Here, input Dark Blue: #2D386D for a unified look.
        5. Drag Order Quantity and Product Weight fields from the Sales table into the Tooltips field well.
        6. Upon selecting the ellipsis at the visualization's top right corner, select the Sort 
           axisdropdown, followed by Sum of Order Total. Then select Sort ascending to sort the values in 
           ascending order.
        7. Observe the column chart results and note the Product Category with the lowest Order Total 
           value. The Order Total for Kids Bikes is $500, making it the product category with the lowest 
           overall sales
* Step 4 : Add the third visual:
        
        1. Select the canvas's empty space to deselect the column chart. Now, select the Line chart icon 
           in the Visualizations pane. An empty line chart will appear on the canvas.
        2. Drag OrderDate from the Sales table into the X-Axis well.
        3. Then, drag Order Total and put it in the Y-Axis well.
        4. You will notice the OrderDate appearing too cramped. To fix this, select the edges of the Line 
           chart visualization box on your canvas to resize it, and place it in the middle of the canvas, 
           below the column chart, next to the table visualization.
* Step 5 : Create KPIs:
   
      1. Ensuring that nothing is selected on the canvas, select the KPI icon in the Visualizations pane. An empty KPI 
         chart will appear on the canvas.
      2. Drag Order Total from the Sales table to the Value field well.
      3. Then drag OrderDate from the Sales table to the Trend Axis field well.
      4. Repeat steps 1 – 3, adding two more KPIs:
         a) Drag Customer ID from the Customers table to the Indicator field well and the OrderDate from the Sales 
            table to the Trend Axis. This will count the number of unique customers that have made a purchase with 
            Adventure Works.
         b) Drag City from the Customers table to the Indicator field well and the OrderDate from the Sales table 
            to the Trend Axis. This will count the number of unique countries that Adventure Works customers are 
            located in.
- Step 6: Setup forecasting:

      1. The first step is to select the line chart visualization you've created. This will bring up the 
         related options in the Visualizations pane on the right-hand side of your Power BI workspace.
      2. You'll notice different tabs in the Visualizations pane, namely Fields, Format, and Analytics. Select the 
         Analytics tab, represented by a magnifying glass icon.
      3. There are a variety of options for adding analytical information to your chart in the Analytics pane.
          Locate the Forecast option and toggle the switch beside it. This will add a forecast line to your chart
      4. Once you've added the forecast, you need to adjust several parameters, such as Seasonality and Confidence 
         interval.
            a) Seasonality: This is useful if your data has a repeating pattern. For the Adventure Works sales
               dataset, setting this to 12 is useful to account for monthly seasonality.
            b) Confidence interval: This is usually set at 95% by default, however you want to ensure the forecast 
               is as confident as possible. Adjust the value to 99%.
      5. Once you've configured the parameters, select Apply to apply the changes. A forecasted line will appear on
         your line chart, in a different color with shading to indicate the confidence intervals.
      6. Observe the line chart and take note of day of the month with the lowest order total for Q1 in 2023. Your 
         analysis shows that the Order Total for March 27th is $200, making it the day with the lowest sales.

- Step 7 :  Configure Q&A:

      1. On the right-hand side of the Power BI Desktop in the Visualizations pane, locate and select the Q&A icon
         that looks like a chat bubble.
      2. Upon selecting the Q&A icon, a Q&A visual will appear on the canvas. The initial size of the Q&A box may
         not fit your needs. Select and drag the corners to resize the box and select and drag the title bar to 
         reposition it on the left side of your canvas.
      3. Inside the Q&A box is a text prompt titled Ask a question about your data. Select inside this box, type the
         following queries, and note down the results:
         A) Which customer City has the lowest average Order Total?
            Long Beach has the lowest average Order Total at $1,200.
         B) Which Product Category has the highest average Order Quantity?
            BMX Bikes have the highest average Order Quantity at 2.00.
         C) Which Product Subcategory has the highest Product Weight?
            The Downhillsubcategory has the highest Product Weight, registering at 151ounces.

# Insights

A single page report was created on Power BI Desktop.

Following inferences can be drawn from the Report.

### [1] Th Total Order from 28 Jan up to 6 Apr 2023 was $6.8 K.
### [2] Number of Customers in this period are 48.
### [3] The Order City for this period are 14.
### [4] We can see that Touring Bikes, Road Bikes, and Mountain Bikes are doing well but we need to focus on marketing plan for Kids Bikes, BMX Bikes, and Hybrid Bikes.
### [5] The line chart showen the stability of the Orders.
