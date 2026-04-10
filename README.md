# Advanced SQL Analytics — Business Intelligence & KPI Reporting
A structured collection of advanced SQL scripts demonstrating end-to-end data analysis across a relational sales database. Covers database exploration, time-series analysis, cumulative metrics, year-over-year performance comparisons, customer segmentation, and analytical reporting — all using production-level SQL techniques.
  * Tools used: SQL Server, GitHub
  * Techniques: Window functions (RANK, LAG, SUM OVER), CTEs, data segmentation, KPI development, YoY/MoM analysis

## 📊 Project Overview

This project is a professional collection of advanced SQL scripts designed to demonstrate real-world data analytics skills.  
The repository focuses on practical business analysis scenarios such as data exploration, KPI reporting, customer analytics, time-series analysis, and performance tracking.

The goal of this project is to show how raw transactional data can be transformed into meaningful insights using structured SQL queries and analytical techniques.

---

## 📁 Datasets Used

This project is built using a range of structured sales/transaction datasets containing information about:

- Customers  
- Products  
- Orders  
- Sales transactions  
- Dates and time-based activity  

You can view or download the datasets here:

👉 [View Datasets](https://github.com/SamofDatasets/advanced-sql-data-analytics/tree/main/datasets)

---

## ⚙️ Database Setup

The project begins by setting up a clean analytical environment.

### 📌 Initialize Database and Schema
**Description:**  
This script creates a new database called `DataWarehouseAnalytics`.  
If the database already exists, it is dropped and recreated to ensure a clean setup.  
A schema named `gold` is also created for analytical queries.

**View Script:**  
👉 [initialize_database.sql](https://github.com/SamofDatasets/advanced-sql-data-analytics/blob/main/scripts/00_init_database.sql)

---

## 🔎 SQL Analysis Scripts

Below is a structured collection of SQL scripts used to explore, analyse, and extract insights from the dataset.

---

### 1. Database Exploration
**Description:**  
Explores the structure of the database, including tables, schemas, and metadata.  
This helps in understanding how the data is organised before performing analysis.

**Skills Demonstrated:**  
Metadata queries, table inspection, schema exploration  

**View Script:**  
👉 [database_exploration.sql](https://github.com/SamofDatasets/advanced-sql-data-analytics/blob/main/scripts/01_database_exploration.sql)

---

### 2. Dimension Tables Exploration
**Description:**  
Explores dimension tables to understand key attributes such as customers, products, and categories.

**Skills Demonstrated:**  
DISTINCT, ORDER BY, exploratory data analysis  

**View Script:**  
👉 [dimensions_exploration.sql](https://github.com/SamofDatasets/advanced-sql-data-analytics/blob/main/scripts/02_dimensions_exploration.sql)

---

### 3. Date Range Exploration
**Description:**  
Determines the earliest and latest dates in the dataset to understand the time coverage of the data.

**Skills Demonstrated:**  
MIN(), MAX(), DATEDIFF(), time-based analysis  

**View Script:**  
👉 [date_range_exploration.sql](https://github.com/SamofDatasets/advanced-sql-data-analytics/blob/main/scripts/03_date_range_exploration.sql)

---

### 4. Measures Exploration (Key Metrics)
**Description:**  
Calculates overall metrics such as total sales, total orders, and average values to provide quick insights into the dataset.

**Skills Demonstrated:**  
COUNT(), SUM(), AVG(), aggregation  

**View Script:**  
👉 [measures_exploration.sql](https://github.com/SamofDatasets/advanced-sql-data-analytics/blob/main/scripts/04_measures_exploration.sql)

---

### 5. Magnitude Analysis
**Description:**  
Analyses how data is distributed across different categories such as products, customers, or regions.

**Skills Demonstrated:**  
GROUP BY, ORDER BY, aggregation  

**View Script:**  
👉 [magnitude_analysis.sql](https://github.com/SamofDatasets/advanced-sql-data-analytics/blob/main/scripts/05_magnitude_analysis.sql)

---

### 6. Ranking Analysis
**Description:**  
Ranks products or customers based on performance metrics to identify top performers and low performers.

**Skills Demonstrated:**  
RANK(), DENSE_RANK(), ROW_NUMBER(), TOP  

**View Script:**  
👉 [ranking_analysis.sql](https://github.com/SamofDatasets/advanced-sql-data-analytics/blob/main/scripts/06_ranking_analysis.sql)

---

### 7. Change Over Time Analysis
**Description:**  
Tracks trends and performance changes over time to identify growth patterns and seasonality.

**Skills Demonstrated:**  
DATEPART(), DATETRUNC(), aggregation, time-series analysis  

**View Script:**  
👉 [change_over_time.sql](https://github.com/SamofDatasets/advanced-sql-data-analytics/blob/main/scripts/07_change_over_time_analysis.sql)

---

### 8. Cumulative Analysis
**Description:**  
Calculates running totals and cumulative metrics to track long-term performance.

**Skills Demonstrated:**  
SUM() OVER(), AVG() OVER(), window functions  

**View Script:**  
👉 [cumulative_analysis.sql](https://github.com/SamofDatasets/advanced-sql-data-analytics/blob/main/scripts/08_cumulative_analysis.sql)

---

### 9. Performance Analysis (YoY & MoM)
**Description:**  
Compares performance across different time periods such as Year-over-Year and Month-over-Month.

**Skills Demonstrated:**  
LAG(), CASE statements, window functions  

**View Script:**  
👉 [performance_analysis.sql](https://github.com/SamofDatasets/advanced-sql-data-analytics/blob/main/scripts/09_performance_analysis.sql)

---

### 10. Data Segmentation Analysis
**Description:**  
Segments customers and products into meaningful groups to support targeted business insights.

**Skills Demonstrated:**  
CASE statements, GROUP BY, segmentation logic  

**View Script:**  
👉 [data_segmentation_analysis.sql](https://github.com/SamofDatasets/advanced-sql-data-analytics/blob/main/scripts/10_data_segmentation.sql)

---

### 11. Part-to-Whole Analysis
**Description:**  
Compares the contribution of different categories to the overall performance.

**Skills Demonstrated:**  
SUM() OVER(), percentage calculations  

**View Script:**  
👉 [part_to_whole_analysis.sql](https://github.com/SamofDatasets/advanced-sql-data-analytics/blob/main/scripts/11_part_to_whole_analysis.sql)

---

## 📊 Analytical Reports

---

### 12. Customer Report
**Description:**  
This report consolidates key customer metrics and behaviours into a single analytical view.

**Key Insights Included:**
- Total orders per customer  
- Total sales and total quantity purchased  
- Customer segmentation (VIP, Regular, New)  
- Recency analysis  
- Average order value  
- Customer lifespan  

**View Script:**  
👉 [customer_report.sql](https://github.com/SamofDatasets/advanced-sql-data-analytics/blob/main/scripts/12_report_customers.sql)

---

### 13. Product Report
**Description:**  
This report provides a complete performance summary for products.

**Key Insights Included:**
- Total sales per product  
- Total quantity sold  
- Product performance segmentation  
- Unique customers per product  
- Recency analysis  
- Average revenue per order  

**View Script:**  
👉 [product_report.sql](https://github.com/SamofDatasets/advanced-sql-data-analytics/blob/main/scripts/13_report_products.sql)

---

## 🧠 Skills Demonstrated in This Project

- Advanced SQL Query Writing  
- Window Functions  
- Data Cleaning & Exploration  
- KPI Development  
- Customer Analytics  
- Time-Series Analysis  
- Business Intelligence Queries  
- Analytical Thinking with SQL  

---

## 🛠 Tools Used

- SQL (SQL Server / PostgreSQL / MySQL compatible queries)
- GitHub
- Relational Databases

---

## 🎯 Project Objective

The objective of this project is to demonstrate strong SQL skills for real-world data analytics roles by transforming raw transactional data into structured business insights.

This repository is part of my data analytics portfolio and reflects practical experience in writing efficient, scalable SQL queries.

---
