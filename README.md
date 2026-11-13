# E-Commerce Sales and Customer Analytics Using Power BI

## Project Overview

This project focuses on analyzing e-commerce sales and customer data using Microsoft Power BI. The objective is to transform raw data into meaningful business insights by studying sales performance, customer purchasing behaviour, product performance, and order trends.

The project uses interactive dashboards to help understand business performance and identify opportunities for improvement.

## Tools and Technologies

- **Microsoft Power BI** – Dashboard development and data visualization
- **Power Query** – Data cleaning and transformation
- **DAX (Data Analysis Expressions)** – Calculated measures and KPIs
- **Data Modeling** – Creating relationships between multiple tables

## Dataset Description

The project uses four main tables:

| Table | Description |
|---|---|
| Customers | Customer details and signup information |
| Products | Product names, categories, prices, and stock |
| Orders | Order dates, payment methods, cities, and order statuses |
| Order_Items | Product quantities and unit prices for each order |

## Project Workflow

1. **Data Preparation:** Imported the datasets into Power BI and used Power Query to inspect data types, missing values, and data quality.
2. **Data Transformation:** Cleaned and prepared the data for analysis.
3. **Data Modeling:** Established relationships between Customers, Products, Orders, and Order_Items tables. Created a Date table for time-based analysis.
4. **DAX Measures:** Developed measures to calculate important business KPIs.
5. **Dashboard Development:** Created interactive dashboards to analyze different areas of e-commerce performance.
6. **Business Insights:** Interpreted dashboard findings and developed recommendations based on the analysis.

## Key DAX Measures

Some of the important measures developed in this project include:

- Total Revenue
- Total Orders
- Average Order Value (AOV)
- Total Customers
- Repeat Customers
- Repeat Rate
- Total Quantity Sold
- Delivered Orders
- Cancelled Orders
- Delivery Rate
- Cancellation Rate

Example – Total Revenue:

```dax
Total Revenue =
SUMX(
    Order_Items,
    Order_Items[quantity] * Order_Items[unit_price]
)
```

Example – Average Order Value:

```dax
AOV =
DIVIDE(
    [Total Revenue],
    [Total Orders]
)
```

## Dashboard Pages

The report contains six interactive dashboards:

### 1. Sales Performance Dashboard
- Analyzed total revenue, order volume, and average order value.
- Identified monthly sales trends.
- Compared revenue across product categories, products, and cities.

### 2. Customer Analytics Dashboard
- Analyzed total customers and ordering customers.
- Examined repeat customer behaviour and customer revenue.
- Compared customer activity across cities.
- Studied customer signup trends.

### 3. Product and Category Performance Dashboard
- Identified high-revenue product categories.
- Compared product sales quantities and revenue.
- Analyzed top-performing and low-performing products.
- Reviewed product stock levels and average product prices.

### 4. Orders and Payments Dashboard
- Analyzed order statuses and payment methods.
- Compared revenue across payment methods.
- Evaluated delivery and cancellation rates.
- Studied order trends over time.

### 5. Customer Value and Retention Dashboard
- Identified customers contributing the highest revenue.
- Analyzed repeat customers and repeat purchase rates.
- Examined average orders and revenue per customer.
- Compared repeat customer activity across cities.

### 6. Executive Summary Dashboard
- Presented key business KPIs in one view.
- Summarized revenue trends, category performance, top products, and city-wise sales.
- Provided an overall view of business performance.

## Key Business Insights

- **Category Performance:** Electronics generated the highest revenue among the product categories analyzed.
- **City Performance:** Mumbai recorded the highest revenue, while Ahmedabad recorded the lowest.
- **Low-Performing Products:** Identified the ten products with the lowest revenue for further evaluation and targeted marketing.
- **Pricing Opportunity:** Recommended testing a potential 4–5% price increase for the highest-selling product while monitoring customer demand and sales volume.
- **Customer Retention:** Analyzed repeat purchasing behaviour to understand customer retention and revenue contribution.

## Business Recommendations

- Strengthen marketing campaigns in cities with lower revenue.
- Use targeted promotions and discounts to improve the performance of low-revenue products, where commercially viable.
- Evaluate pricing opportunities for high-performing products through controlled testing.
- Encourage repeat purchases through customer engagement and retention initiatives.
- Monitor cancellation trends and payment methods to identify areas for operational improvement.

## Skills Demonstrated

- Data Cleaning and Transformation
- Data Modeling
- DAX Calculations
- KPI Development
- Data Analysis
- Interactive Dashboard Development
- Business Intelligence
- Data Visualization
- Business Insights and Recommendations

## Conclusion

This project helped me gain practical experience in using Power BI to analyze e-commerce data and convert it into actionable business insights. It strengthened my understanding of data preparation, data modeling, DAX calculations, dashboard development, and business analysis.
