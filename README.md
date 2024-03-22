# Data-Analytics-Projects
### 1. [Super mart dashboard visual](https://github.com/puru0001/Data-Analytics-Projects/tree/main/superstore%20data)
![SuperMart Dashboard visual.](/Src/images/supermart_1.jpg "SuperMart Dashboard visual 1.")

![SuperMart Dashboard visual.](/Src/images/supermart_2.jpg "SuperMart Dashboard visual 2.")

![SuperMart Dashboard visual.](/Src/images/supermart_3.jpg "SuperMart Dashboard visual 3.")

It displays various sales and profit metrics for a fictional company, Super Mart. While Power BI itself doesn’t use Excel formulas directly, it uses a similar formula language called DAX (Data Analysis Expressions) to create calculated columns and measures.

Here’s a breakdown of the different sections of the dashboard and the kind of DAX formulas that could be used to create them:

#### Sales by Month

This is a line chart that shows the total sales per month throughout the year. A DAX formula would be used to calculate the total sales for each month. This would likely involve summing the sales amount for each transaction record where the transaction date falls within the specified month.

#### Number of Orders by Ship Mode

This is a pie chart that shows the number of orders shipped by each shipping method (First Class, Same Day, Standard Class). A DAX formula would be used to calculate the count of orders for each ship mode. This would likely involve filtering the data for each ship mode and then using the COUNTROWS function to count the number of records in the filtered table.

#### Sales by Category

* This section breaks down total sales into two parts: a stacked bar chart that shows sales by category (Office Supplies, Technology, Furniture) for each month, and a donut chart that shows the percentage of total sales for each category.

* The stacked bar chart would likely use a combination of DAX formulas to calculate sales by category and month. One formula would be used to filter the data for each category and month. Another formula would be used to sum the sales amount for the filtered data.

* The donut chart would use a DAX formula to calculate the total sales for each category. This would likely involve summing the sales amount for each transaction record where the product category matches the specified category. Then another formula would be used to calculate the percentage of total sales for each category by dividing the category sales total by the grand total sales and formatting the result as a percentage.

#### Sales and Profit by Year

This section displays a line chart showing the sum of sales and sum of profit for each year. DAX formulas would be used to calculate the total sales and total profit for each year. This would likely involve filtering the data for each year and then using the SUMX function to sum the sales amount and profit amount for the filtered data.

#### Profit by Top Product

This section shows a bar chart that displays the profit earned from each of the top profit-generating products. A DAX formula would be used to calculate the profit for each product. This would likely involve subtracting the cost of goods sold from the sales amount for each transaction record, and then summing the profit amount for each product. The products would then be sorted by profit, showing the top products.

#### Quantity by Category

* This section displays a bar chart showing the total quantity sold for each product category. A DAX formula would be used to calculate the total quantity sold for each category. This would likely involve summing the quantity sold for each transaction record where the product category matches the specified category.

* It’s important to note that these are just examples of how DAX formulas could be used to create the visuals in this dashboard. The specific formulas would depend on the structure of the underlying data in Power BI.

### 2. [Ecommerce Sales Dashboard](https://github.com/puru0001/Data-Analytics-Projects/tree/main/Ecom)

![e commerce Dashboard visual.](/Src/images/e_com_1.jpg "e commerce Dashboard visual 1.")

![e commerce Dashboard visual.](/Src/images/e_com_2.jpg "e commerce Dashboard visual 2.")

![e commerce Dashboard visual.](/Src/images/e_com_3.jpg "e commerce Dashboard visual 3.")

It displays various sales and profit metrics for an e-commerce business. While Power BI itself doesn't use Excel formulas directly, it uses a similar formula language called DAX (Data Analysis Expressions) to create calculated columns and measures. SQL is used to query relational databases and retrieve data for use in Power BI.

Here’s a breakdown of the different sections of the dashboard and the kind of DAX formulas that could be used to create them:

* Qtr 1 - Qtr 4 & All: This section likely uses a slicer to allow users to filter the data by quarter.

* Profit by Month: This section likely uses a DAX formula to calculate the total profit for each month. This would likely involve summing the profit amount for each transaction record where the transaction date falls within the specified month.

#### Sum of Profit & Average of Amount: 
These are most likely measures created with DAX formulas.
  * Sum of Profit: This would likely involve summing the profit amount for all transactions.
  * Average of Amount: This would likely involve calculating the average of the sales amount for all transactions.

#### Amount by State: 
This section likely shows a table that breaks down the total sales amount by state. A DAX formula would be used to calculate the total sales for each state. This would likely involve summing the sales amount for each transaction record where the customer’s state matches the specified state.

#### Quantity by Category: 
This section likely shows a bar chart that displays the total quantity sold for each product category. A DAX formula would be used to calculate the total quantity sold for each category. This would likely involve summing the quantity sold for each transaction record where the product category matches the specified category.

#### Amount by CustomerName: 
This section likely shows a table that breaks down the total sales amount by customer name. A DAX formula would be used to calculate the total sales for each customer. This would likely involve summing the sales amount for each transaction record where the customer name matches the specified customer name.

#### Quantity by Payment Mode: 
This section likely shows a pie chart that shows the number of orders placed using each payment method (EMI, COD, Credit Card, Debit Card, UPI). A DAX formula would be used to calculate the count of orders for each payment mode. This would likely involve filtering the data for each payment mode and then using the COUNTROWS function to count the number of records in the filtered table.

#### Profit by Sub-Category: 
This section likely shows a table that breaks down the total profit by product subcategory. A DAX formula would be used to calculate the total profit for each subcategory. This would likely involve subtracting the cost of goods sold from the sales amount for each transaction record, and then summing the profit amount for each subcategory.

- It’s important to note that these are just examples of how DAX formulas could be used to create the visuals in this dashboard. The specific formulas would depend on the structure of the underlying data in Power BI.

### 3. [HR Data Dashboard](https://github.com/puru0001/Data-Analytics-Projects/tree/main/Hr%20DA)

![Hr data Dashboard visual.](/Src/images/Hr_dashboard.png "Hr data Dashboard visual 1.")

Tableau uses its own calculation language called Tableau Calculation Language (TCL) to create calculated fields and measures. It does not directly use Excel formulas.

The dashboard you sent appears to be a CEO dashboard that displays KPIs (Key Performance Indicators) related to project execution and budget. Here’s a breakdown of the different sections of the dashboard and the kind of Tableau Calculation Language (TCL) expressions that could be used to create them:

#### Budget Sought vs. Approved vs. Required

This section likely displays three measures created with TCL expressions:
    * Budget Sought: This would likely sum the amount of budget requested across all projects.
    * Budget Approved: This would likely sum the amount of budget approved across all projects.
    * Budget Required: This could be another measure that calculates the current amount of budget needed to complete projects.

#### Execution Status

This section likely uses a stacked bar chart to show the count of projects in different execution states (On Track, Delayed, Complete, Not Yet Started, Risk of Delay, Unavailable). A TCL calculation would be used to determine the execution status for each project and then a calculated field could be created to bin the projects into the different execution status categories. Finally, a measure would be created to count the number of projects in each category.

#### Project Status by Category

This section likely uses a heat map to show the count of projects in different categories (Coal, Water, Fly Ash, etc.) across different project statuses (Complete, Delayed, On Track, Risk of Delay). Similar to the “Execution Status” section, TCL calculations would be used to determine the project status and category for each project, and then a calculated field could be created to assign each project to a cell in the heat map. Finally, a measure would be created to count the number of projects in each cell.

#### Budget by Project Level

This section likely shows a table that breaks down the budget by project level (Departmental, Programmatic). A TCL calculation would likely be used to determine the project level for each project, and then a measure would be created to sum the budget amount for each project level.

#### Start and End Dates

This section likely displays the earliest start date and the latest end date out of all the projects. Tableau has built-in functions to find minimum and maximum values. A TCL calculation could be used to determine the start and end date for each project, and then the MIN and MAX functions could be used to find the overall minimum start date and maximum end date.

It’s important to note that these are just examples of how Tableau Calculation Language (TCL) expressions could be used to create the visuals in this dashboard. The specific calculations would depend on the structure of the underlying data in Tableau.


### 4. [SQL Murder Mystery](https://github.com/puru0001/Data-Analytics-Projects/blob/main/SQL%20Murder%20Mystery%20soln.pdf)

![SQL Murder Mystery.](/Src/images/SQL_murder_myster.jpg "SQL Murder Mystery")

Thish is the Schema of SQL Murder mystery.
![SQL Murder Mystery schema.](/Src/images/Murder_mys_schema.png "SQL Murder Mystery Schema")

I have solved the knight lab's SQL murder mystery problem the whole approach is documented.
fore more details reach out the knight lab website and solve the mystery.
click here : [knight lab](https://mystery.knightlab.com/).