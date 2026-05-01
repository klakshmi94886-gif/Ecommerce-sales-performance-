# Ecommerce-sales-performance-
excel project
Ecommerce Sales Analysis: Data Cleaning, Analysis & Visualization


📊 Project Overview
This project involves a comprehensive analysis of an e-commerce transactional dataset using Microsoft Excel. The goal was to transform raw sales data into an interactive dashboard to identify sales trends, regional performance, and customer payment preferences.

🎯 Project Objectives

•	Sales Trends (Line Chart): Plot Total_Amount against Order_Date (grouped by Month) to identify seasonal peaks or declining trends.
•	Category Performance (Pie or Donut Chart): Show the distribution of sales across categories like Electronics, Clothing, or Home.
•	Regional Analysis (Clustered Column Chart): Compare how different regions (North, South, East, West) are performing against each other.
•	Top 5 Products (Bar Chart): Use a horizontal bar chart to rank the highest revenue-generating products.


🛠️ Data Processing Workflow

1. Data Entry & Organization
   

•	Import Data: Use the provided E-commerce store dataset link. Go to the Data tab in    Excel and use Get Data to import your file.
•	Table Conversion: Select your data range and press Ctrl + T to convert it into an official Excel Table. Name your table (e.g., SalesData) in the Table Design tab.
•	Data Types: Ensure the "Date" column is formatted as a Date, "Price/Revenue" as Currency,    and "Quantity" as a Number
•	Text: Use PROPER() or UPPER() to fix inconsistent capitalization in product names.

2. Data Cleaning
•	Missing Values: Some rows have missing discounts or totals (e.g., SALE26, SALE52, SALE64, SALE70, SALE94). These need correction or imputation.
•	Erroneous Records: Certain rows show inconsistencies (e.g., SALE19 has Unit_Price = 0.04 but Total_Amount = 1782.45).
•	Duplicates: Check for duplicate Sales_ID entries.
•	Date Conversion: Order_Date values are numeric and should be converted into proper date format using Excel’s DATE or TEXT functions.
•	Handle Missing Data: Use Find & Select > Go To Special > Blanks to identify empty cells. 
•	Irrelevant Data: Scan for columns that do not contribute to analysis  delete them.
•	Combining Tables: If your data is split into "Orders" and "Products," use XLOOKUP or VLOOKUP to bring product prices into the order table.

3. Analysis & Formulas
Calculations were performed using the following logic:
•	Revenue Calculation: Formula: =Quantity * Unit_Price * (1 - Discount)
•	Discount Amount: Formula: =Quantity * Unit_Price * Discount
•	Payment Type Summary: Use SUMIF or COUNTIF to calculate totals by payment method.
•	Customer/Product Lookup: Use VLOOKUP or XLOOKUP to merge with customer/product tables (if available).
•	Logical: Use =IF(Sales > 1000, "High", "Low") to categorize orders.

📈 Descriptive Statistics
The Total_Amount sales metric was analyzed using the Excel Analysis 
ToolPak:  
Metric        Value 
Sum           2,173,935  
Mean          1,086.97  
Median          868.72  
Standard Dev.   818.85  
Skewness          0.88  
Count         2,000 records 

 Pivot Table Analysis
•	Revenue by Payment Type: Compare Credit Card, PayPal, COD.
•	Revenue by Store: Identify top-performing stores.
•	Top Products: Rank products by total sales
💡 Key Insights
Payment Preferences: PayPal is the dominant payment method, followed by Credit Cards and COD.  
Top Performers: Stores 8, 12, and 17 drive the highest sales volumes. 
Product Leaders: Products like PROD33 and PROD49 are top revenue generators. 
Skewed Distribution: The mean is higher than the median, indicating that high-value bulk orders are pulling the average up

🖼️ Dashboard Preview
The final Excel Dashboard includes:

1. Line Chart: Monthly Revenue Trends.
2. Clustered Column Chart: Regional Performance Comparison.  
3. Pie Chart: Revenue Share by Payment Method. 
4. Slicers: Interactive filtering by Store, Product, and Payment Type.
   
📂 File Structure
Raw Data: Original unedited dataset.  
Cleaned Data: Dataset after handling missing values and errors.  
Pivot Tables: Summarized data for visualization. 
Dashboard: Interactive visual representation.
Date Normalization: Converted numeric Order_Date values into readable date formats. 
Text Cleaning: Used PROPER() functions to fix inconsistent capitalization in product names.
