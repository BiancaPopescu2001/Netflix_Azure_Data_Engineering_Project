# Netflix Azure Data Engineering Project

[![Text](https://github.com/BiancaPopescu2001/Netflix_Azure_Data_Engineering_Project/blob/main/cover.jpg))


## TABLE OF CONTENT
- [Introduction](#introduction)
- [Sales Dashboard | Requirements](#sales-dashboard--requirements)
  - [Dashboard Purpose](#dashboard-purpose)
  - [Key Requirements](#key-requirements)
    - [KPI Overview](#kpi-overview)
    - [Sales Trends](#sales-trends)
    - [Product Subcategory Comparison](#product-subcategory-comparison)
    - [Weekly Trends for Sales & Profit](#weekly-trends-for-sales--profit)
- [Skills demonstrated](#skills-demonstrated)
- [Data Dictionary](#data-dictionarry)
- [Data Modelling](#dat-amodelling)
- [Analysis](#analysis)
- [Dashboard Link](#dashboard-link)
- [Conclusion](#conclusion)
  


## Introduction
This user story outlines the specifications for building two dashboards using Tableau to help stakeholders, including sales managers and executives to analyze sales performance and customers.

## Sales Dashboard | Requirements

### Dashboard Purpose
The purpose of Sales Dashboard is to present an overview of the sales metrics and trends in order to analyze year-over-year sales performance and understand sales trends.

### Key Requirements

#### KPI Overview
Display a summary of total sales, profits and quantity for the current year and the previous year

#### Sales Trends
-	Present the data for each KPI on a monthly basis for both the current year and the previous year.
-	Identify months with highest and lowest sales and make them easy to recognize.

#### Product Subcategory Comparison
-	Compare sales performance by different product subcategories for the current year and the previous year.
-	Include a comparison of sales with profit.

#### Weekly Trends for Sales & Profit
-	Present weekly sales and profit data for the current year.
-	Display the average weekly values.
-	Highlight weeks that are above and below the average to draw attention to sales & profit performance.

## Skills Demonstrated
- Data Visualization
- Dashboard Design
- Analytical Thinking / Problem Solving
- Storytelling with Data
- Trend & Pattern Analysis

## Data Dictionary

1. **Customers** - Each row represents a unique customer on the platform

<table>
  <tr>
    <th>Field Name</th>
    <th>Type</th>
    <th>Description</th>
    <th>Example</th>
  </tr>
  <tr>
    <td>Customer ID</td>
    <td>STRING</td>
    <td>Unique ID for each user</td>
    <td>AA-10315</td>
  </tr>
  <tr>
    <td>Customer Name</td>
    <td>STRING</td>
    <td>User’s full name</td>
    <td>Alex Avila</td>
  </tr>
</table>

2. **Orders** - Each row represents an order placed by customer

<table>
  <tr>
    <th>Field Name</th>
    <th>Type</th>
    <th>Description</th>
    <th>Example</th>
  </tr>
  <tr>
    <td>Order ID</td>
    <td>STRING</td>
    <td>Unique ID for each order</td>
    <td>CA-2022-152156</td>
  </tr>
  <tr>
    <td>Order Date</td>
    <td>Date</td>
    <td>The date when the order was placed by the customer</td>
    <td>08.11.2022</td>
  </tr>
  <tr>
    <td>Customer ID</td>
    <td>STRING</td>
    <td>Unique ID of the user who placed the order</td>
    <td>CG-12520</td>
  </tr>
   <tr>
    <td>Product ID</td>
    <td>STRING</td>
    <td>Unique ID of the product ordered by user</td>
    <td>FUR-BO-10001798</td>
  </tr>
   <tr>
    <td>Sales</td>
    <td>FLOAT</td>
    <td>Total cost of the order</td>
    <td>261,96</td>
  </tr>
   <tr>
    <td>Quantity</td>
    <td>INTEGER</td>
    <td>Total number of articles for each product ordered by customer</td>
    <td>2</td>
  </tr>
  <tr>
    <td>Profit</td>
    <td>FLOAT</td>
    <td>Total profit of the order</td>
    <td>41,9136</td>
  </tr>
</table>

3. **Products** - Each row represents an unique product from the platform

<table>
  <tr>
    <th>Field Name</th>
    <th>Type</th>
    <th>Description</th>
    <th>Example</th>
  </tr>
    <td>Product ID</td>
    <td>STRING</td>
    <td>Unique ID for each product</td>
    <td>FUR-BO-10000112</td>
  </tr>
  <tr>
    <td>Category</td>
    <td>STRING</td>
    <td>Group that classifies a product based on its type, use, or characteristics</td>
    <td>Furniture</td>
  </tr>
   <tr>
    <td>Sub-Category</td>
    <td>STRING</td>
    <td>Specific classification within a category</td>
    <td>Furniture</td>
  </tr>
  <tr>
    <td>Product Name</td>
    <td>STRING</td>
    <td>Unique name for each product</td>
    <td>O'Sullivan 2-Shelf Heavy-Duty Bookcases</td>
  </tr>
</table>

## Data Modelling

The main orders table was related to the customers info and products tables using the Order ID, Customer ID columns

![Data Modelling](https://github.com/BiancaPopescu2001/Tableau/blob/298dd4b73161beb4d60189eb4c01f1a27948ab98/data%20modelling.png)


## Analysis
2023 outperformed 2022 in all key metrics (sales, profit, and quantity).

Profitability is not evenly distributed — some high-revenue subcategories underperform in terms of profit.

The final quarter shows a noticeable upward trend, suggesting effective seasonal strategies or increased demand.


## Dashboard Link

https://public.tableau.com/app/profile/bianca.popescu/viz/SalesDashboard_17612430350950/SalesDashboard

## Conclusion

Future strategies should focus on improving margins in low-profit categories while maintaining sales growth momentum.
