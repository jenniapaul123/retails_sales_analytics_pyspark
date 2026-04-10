# Retail Sales Analytics using PySpark

## 📌 Overview
This project analyzes large-scale online retail transaction data using PySpark to identify key business insights such as revenue trends, top-selling products, high-value customers, and country-level performance.

The project demonstrates how big data tools like Spark can be used to process and analyze large datasets efficiently in a scalable manner.

## 🎯 Business Problem
Retail businesses generate large volumes of transaction data. This project aims to:
- Identify top-performing products
- Analyze customer purchasing behavior
- Understand revenue trends over time
- Evaluate country-level sales performance
- Detect seasonal patterns in sales

## 🛠️ Technologies Used
- Python
- PySpark (Spark DataFrames & Spark SQL)
- Jupyter Notebook
- Matplotlib
  
## 📂 Dataset
- **Source:** UCI Online Retail Dataset
- **Size:** ~500,000+ transaction records
- **Key Columns:**
  - InvoiceNo
  - StockCode
  - Description
  - Quantity
  - InvoiceDate
  - UnitPrice
  - CustomerID
  - Country

## ⚙️ Project Workflow

### 1. Data Loading
- Loaded CSV data into PySpark DataFrame

### 2. Data Cleaning
- Removed cancelled transactions
- Filtered out invalid values (negative quantity/price)
- Handled missing values

### 3. Feature Engineering
- Created `Revenue` column (Quantity × UnitPrice)
- Extracted year and month from InvoiceDate

### 4. Data Analysis
- Total revenue calculation
- Top products by revenue and quantity
- Top customers by revenue
- Country-wise revenue analysis
- Monthly sales trends

### 5. Advanced Spark Operations
- Aggregations using `groupBy`
- Multi-dimensional analysis using `rollup`, `cube`
- Pivot table for country-level monthly sales
- Frequent item analysis

### 6. Spark SQL
- Created temporary view and executed SQL queries for analysis

### 7. Visualization
- Monthly revenue trend
- Top countries by revenue
- Top customers and products
