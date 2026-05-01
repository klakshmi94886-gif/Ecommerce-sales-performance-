# Ecommerce-sales-performance-
excel project
Ecommerce Sales Analysis: Data Cleaning, Analysis & Visualization
📊 Project Overview
This project involves a comprehensive analysis of an e-commerce transactional dataset using Microsoft Excel. The goal was to transform raw sales data into an interactive dashboard to identify sales trends, regional performance, and customer payment preferences.
🎯 Project Objectives
Sales Trends: Identify seasonal peaks and declining trends using monthly revenue plots.  

Category Performance: Analyze the distribution of sales across product categories.  

Regional Analysis: Compare performance across North, South, East, and West regions.  

Top 5 Products: Rank the highest revenue-generating products.
🛠️ Data Processing Workflow
1. Data Entry & Organization
Import: Data was imported via the Get Data tool in Excel.  

Table Conversion: Range converted to an official Excel Table (SalesData) for structured referencing.  

Data Types: Standardized formatting for Dates, Currency, and Numbers.
2. Data Cleaning
Missing Values: Addressed null values in discounts and totals (e.g., SALE26, SALE52) using Go To Special > Blanks.  

Erroneous Records: Corrected inconsistencies where Unit_Price did not align with Total_Amount.  
3. Analysis & Formulas
Calculations were performed using the following logic:

Total Revenue: =Quantity * Unit_Price * (1 - Discount)  

Discount Amount: =Quantity * Unit_Price * Discount 

Order Categorization: Used =IF(Sales > 1000, "High", "Low")
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
