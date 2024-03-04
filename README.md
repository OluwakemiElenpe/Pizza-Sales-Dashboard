# Boston Pizza Sales Analysis

![](Pizza.jpg)

## Introduction
This is a power BI project on sales analysis of an imaginary store called **Boston Pizza**. It is a year worth of sales from a fictitious pizza place. The project is to analyze and derive insights to answer crutial questions and help the store make data driven decisions.

_*Disclimer_*: _*All datasets and reports do not represent any company or store.*_

## Recommended Analysis
1.	How many customers do we have each day? Are there any peak hours?
2.	How many pizzas are typically in an order? Do we have any bestsellers?
3.	How much money did we make this year? Can we indentify any seasonality in the sales?
4. Are there any pizzas we should take of the menu, or any promotions we could leverage?

## Skills demostrated
The following Power BI features were incorporated: Data cleaning, Bookmarking, DAX, Modelling, Filters.

## Data gathering
The dataset was downloaded on Maven Analytics website. Here is the link to the [dataset](https://www.mavenanalytics.io/data-playground?dataStructure=2lXwWbWANQgI727tVx3DRC&search=pizza)
It consists of four datasets namely:
- Orders
- Order_details
- Pizzas
- Pizza_types

## Data Transformation/data cleaning
The underscore for the column header was removed. The first row of the pizza types dataset was promoted as row header.

Pizza types before cleaning            |          Pizza types after cleaning
:-------------------------------------:|:----------------------------------------:|
![](Pizza_types_b4_cleaning.png)       |  ![](Pizza_types_after_cleaning.png)

Pizza before cleaning                  |          Pizza after cleaning
:-------------------------------------:|:----------------------------------------:|
![](Pizza_b4_cleaning.png)             |   ![](Pizza_after_cleaning.png)

Order details before cleaning          |          Order details after cleaning
:-------------------------------------:|:------------------------------------------------:|
![](Order_details_b4_cleaning.png)     |   ![](Order_details_after_cleaning.png)

Order before cleaning                  |          Order after cleaning
:-------------------------------------:|:------------------------------------------------:|
![](Order_b4_cleaning.png)             |   ![](Order_after_cleaning.png)


- The datatype for each column header was checked and edited as appropriate. Null value was checked for each column header by checking the column quality. If the valid of each column is less than 100% it means that the row contains Null value. But for the four datasets all the valid values were 100% it means that there is no missing or Null value.

- New measures were created to calculate the total sales, Orders, Average orders in a day, Avg pizzas in an order respectively.

Total Sales                            |          Orders
:-------------------------------------:|:------------------------------------------------:|
![](Total_sales.png)                   |   ![](Orders.png)


Average Order in a day                      |          Average Pizzas in a day
:------------------------------------------:|:------------------------------------------------:|
![](Avg_Order_day.png)                      |   ![](Avg_Pizzas_Order.png)


## Data Modelling

Date table was created using the below code:

![](Date_table.png)

Relationship was created within the five datasets. 

![](Data_Model.png)
The model is a star schema. There are 4-dimension tables and 1 fact table. Order details is the fact table because it contains the quantitative data being analyzed.

## Analysis

Average number of customer             |         Average Pizza in an order
:-------------------------------------:|:------------------------------------------------:|
![](Average_Order.png)                 |   ![](pizza_no.png)

The store has a total number of 21,350 orders and the total is $817,860.
The average order in a day is 60 this implies that the average number of customer in a day is 60. The amount of pizzas typically in an order is two.

Best Seller                            |          Least Seller
:-------------------------------------:|:------------------------------------------------:|
![](Top_5_pizzas.png)                  |   ![](Buttom_5_pizzas.png)

The best seller is the Thia chicken pizza with the total sales of $43,434 while the least pizza is The Brie Carre Pizza with total sales of $11,588 

Sales by Month and Year                |          Peak Hour
:-------------------------------------:|:------------------------------------------------:|
![](Sales_by_month_year.png)           |   ![](Time_slot.png)

The sales shows an up and downward movement it means that the sales wasn't stable throughtout the year. But the month of July has the highest sales of $72,600. 
The peak hour is between 12 - 3pm.
  

Sales by Day                           |          Sales by Size
:-------------------------------------:|:------------------------------------------------:|
![](Sales_by_day.png)                  |   ![](Sales_size.png)

The highest sales of the week is on Friday with total sales of $136,074. The highest sales by size is Large with total sales of $375,319

Sales by Category                      |         
:-------------------------------------:|
![](Sales_Category.png)                |   

The highest sales by category is Classic with total sales of $220,000.

[![](https://github.com/OluwakemiOretade/Pizza-Sales-Dashboard/blob/main/Dashboard.png)](https://app.powerbi.com/view?r=eyJrIjoiYzA5ZTMyYmYtYzYxMS00MzVkLTk1ZTMtZmM5ZWQyNjM4Y2ExIiwidCI6IjVkMTA4NWVkLTYyZDgtNGRhZC05MDI1LWY5YWFiNDIzNDllZSJ9)

![](Dashboard.png) 

## Conclusion
The suggested seasonality period will be the month of July where we have the total sales of $72,000, though further investigation will reveal if there is a special event that occurs in that month. Based on the pizza with the least sales the pizza that should be take off the menu is The Brie Carre Pizza with $11,588 worth of sales. 

## Recommendation
For a deep dive into the analytics, the datasets of the previous years will be required for comparison and data driven decision.
