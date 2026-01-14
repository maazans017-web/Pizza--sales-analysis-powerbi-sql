📌 Project Overview

The Pizza Sales Analysis project is an end-to-end business intelligence solution built using SQL and Power BI. The objective of this project is to analyze pizza sales transaction data to uncover revenue trends, customer demand patterns, and product performance insights that can help a pizza business make data-driven operational and strategic decisions.

This project demonstrates the complete analytics lifecycle — from raw data understanding and cleaning, to data modeling, DAX calculations, visualization, and business insights.

🎯 Business Objective

The key business questions addressed in this project are:

Which pizza categories and sizes generate the highest revenue?

What are the peak sales hours and days?

Which pizzas contribute the most to total sales?

How does sales performance change over time?

The goal is to help the business optimize:

Inventory planning

Staffing decisions

Promotional strategies

Product focus

🗂️ Data Source
The dataset used in this project is a pizza sales transactional dataset, commonly used for retail and BI practice.

📄 Dataset Includes:

Order ID
Order Date
Order Time
Pizza Name
Pizza Category
Pizza Size
Quantity Sold
Unit Price
Total Price

📌 Data Type: Structured CSV files
📌 Granularity: Order line–level data

🧹 Data Cleaning & Preparation

Data cleaning was performed to ensure accuracy and reliability of analysis.

Key Steps:
Removed duplicate order records to avoid double counting revenue
Handled null values:
Removed rows with nulls in critical numeric fields (price, quantity)
Validated category and size values
Ensured correct data types for date, time, and numeric fields
Verified revenue calculations (Quantity × Unit Price)
This step ensured high data quality before loading into Power BI.

🛠️ Tools & Technologies Used

SQL – Data extraction, joins, aggregations, validation
Power BI Desktop – Data modeling, visualization, reporting
DAX (Data Analysis Expressions) – KPI calculations
Excel / CSV – Raw data storage

🧩 Data Modeling

A Star Schema was implemented for efficient reporting and performance.

⭐ Data Model Structure:

Fact Table:

Sales / Orders (transactional data)

Dimension Tables:
Date
Pizza
Pizza Category
Pizza Size

📌 This model improves:

Query performance

DAX calculation simplicity
Scalability for future analysis

📐 DAX Measures Used

The following DAX measures were created to calculate business KPIs:

Total Revenue
SUM(Sales[Total Price])

Total Orders
DISTINCTCOUNT(Sales[Order ID])

Total Quantity Sold
SUM(Sales[Quantity])

Average Order Value (AOV)
DIVIDE([Total Revenue], [Total Orders])

Revenue by Category / Size
Dynamic measures using CALCULATE() and filter context

Top Selling Pizzas
Ranking using RANKX()

Time-Based Analysis
Revenue trends by day, month, and hour

📊 Dashboard & Visualizations

An interactive Power BI dashboard was created to present insights clearly to business stakeholders.

Visuals Included:

KPI Cards:

Total Revenue
Total Orders
Average Order Value
Bar Charts: Revenue by Pizza Category
Top-Selling Pizzas
Line Charts: Daily and monthly revenue trends
Time Analysis Charts: Sales by hour of the day
Slicers: Date
Category
Size

📌 The dashboard allows users to interactively explore data and drill down into specific insights.

🔍 Key Insights

Certain pizza categories and sizes consistently generate higher revenue
Sales peak during specific hours and days, indicating strong demand patterns
A small number of pizzas contribute a significant portion of total revenue
Demand patterns can be used to optimize staffing and inventory planning

📈 Business Impact

Based on the insights:
Inventory can be optimized by focusing on high-demand pizzas
Staffing can be aligned with peak sales hours
Promotions can target top-performing categories
Low-performing items can be reviewed for improvement or removal

✅ Conclusion

This project demonstrates the ability to:
Perform end-to-end data analysis using SQL and Power BI
Build efficient data models and DAX measures
Translate raw transactional data into actionable business insights
Design executive-friendly dashboards for decision-making
The Pizza Sales Analysis project showcases strong fundamentals in Business Intelligence, Data Visualization, and Analytical Thinking, making it suitable for Data Analyst / Power BI roles.


Demo screeonshot : (https://github.com/maazans017-web/Pizza--sales-analysis-powerbi-sql/blob/main/Crazy%20Pizza%20Sales%20Analysis.png)

Pbix File : (https://github.com/maazans017-web/Pizza--sales-analysis-powerbi-sql/blob/main/pizza%20sales%20project.pbix)
