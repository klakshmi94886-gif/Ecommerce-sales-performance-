# Ecommerce-sales-performance-

ECommerce Sales Performance

Excel project: Ecommerce Sales Analysis with Data Cleaning, Analysis, and Visualization.

## 📊 Project Overview

This project analyzes an e-commerce transactional dataset using Microsoft Excel. The goal is to transform raw sales data into a clean dataset and an interactive dashboard that surfaces sales trends, regional performance, and payment preferences.

## 🎯 Project Objectives

- **Sales Trends** (Line Chart): Plot `Total_Amount` against `Order_Date` by month to identify peaks and declines.
- **Category Performance** (Pie or Donut Chart): Visualize sales distribution across categories like Electronics, Clothing, and Home.
- **Regional Analysis** (Clustered Column Chart): Compare performance across North, South, East, and West.
- **Top 5 Products** (Bar Chart): Rank the highest revenue-generating products.

## 🛠️ Data Processing Workflow

### Data Entry & Organization

- Import dataset through Excel: **Data > Get Data**.
- Convert the data range into an Excel Table with `Ctrl + T` and name it `SalesData`.
- Format columns appropriately:
  - `Order_Date` as Date
  - `Unit_Price` and `Total_Amount` as Currency
  - `Quantity` as Number
- Clean text fields using `PROPER()` or `UPPER()` to standardize product names.

### Data Cleaning

- **Missing Values:** Correct or impute missing discounts and totals (for example, rows such as SALE26, SALE52, SALE64, SALE70, SALE94).
- **Erroneous Records:** Fix inconsistent entries, such as `SALE19` having `Unit_Price = 0.04` but `Total_Amount = 1782.45`.
- **Duplicates:** Remove duplicate `Sales_ID` rows.
- **Date Conversion:** Convert numeric `Order_Date` values to actual dates using `DATE()` or `TEXT()`.
- **Blank Cells:** Use **Find & Select > Go To Special > Blanks** to identify missing values.
- **Irrelevant Columns:** Remove any fields not needed for analysis.
- **Lookup Tables:** If data is split across `Orders` and `Products`, use `XLOOKUP()` or `VLOOKUP()` to merge fields.

### Analysis & Formulas

- `Revenue = Quantity * Unit_Price * (1 - Discount)`
- `Discount Amount = Quantity * Unit_Price * Discount`
- Use `SUMIF()` or `COUNTIF()` to summarize by payment type.
- Use `VLOOKUP()` or `XLOOKUP()` to add customer/product details from supporting tables.
- Categorize orders with formulas like `=IF(Total_Amount > 1000, "High", "Low")`.

## 📈 Descriptive Statistics

The `Total_Amount` metric was analyzed using Excel Analysis ToolPak.

| Metric      | Value     |
|-------------|-----------|
| Sum         | 2,173,935 |
| Mean        | 1,086.97  |
| Median      | 868.72    |
| Std Dev     | 818.85    |
| Skewness    | 0.88      |
| Count       | 2,000     |

## 📊 Pivot Table Analysis

- Revenue by Payment Type: Compare Credit Card, PayPal, and COD.
- Revenue by Store: Identify top-performing stores.
- Top Products: Rank products by total sales.

## 💡 Key Insights
    
- **Payment Preferences:** PayPal appears to be the dominant payment method, followed by Credit Card and COD.
- **Top Performers:** Stores 8, 12, and 17 drive the highest sales volumes.
- **Top Products:** Products such as `PROD33` and `PROD49` are top revenue generators.
- **Sales Distribution:** A higher mean than median suggests right-skewed sales due to large orders.

## 🖼️ Dashboard Preview

The final Excel dashboard includes:

- Line Chart: Monthly revenue trends
- Clustered Column Chart: Regional performance comparison
- Pie Chart: Revenue share by payment method
- Slicers: Interactive filters by Store, Product, and Payment Type

## 📂 File Structure

- **Raw Data:** Original unedited dataset
- **Cleaned Data:** Dataset after handling missing values and correcting errors
- **Pivot Tables:** Summaries used for visualization
- **Dashboard:** Interactive visual report
- **Date Normalization:** Converted numeric `Order_Date` values into readable dates
- **Text Cleaning:** Standardized capitalization using `PROPER()`



 
