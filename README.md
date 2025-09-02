# Calzone-Sales-Analysis-Excel
 
## Table of Contents
- [Problem](#problem)
- [Objective](#objective)
- [Dataset Description](#dataset-description)
- [Data Cleaning & Preparation](#data-cleaning--preparation)
- [KPIs Defined](#kpis-defined)
- [Analysis & Visualizations](#analysis--visualizations)
- [Key Insights](#key-insights)
- [Tools & Techniques Used](#tools--techniques-used)
- [Recommendations](#recommendations)

---

## Problem
Alpha Calzone is facing challenges understanding its sales performance across product categories, sizes, and time trends. The management wants to uncover key insights from historical sales data to optimize staffing, improve marketing efforts, and maximize revenue.

---

## Objective
- Clean and prepare the dataset for analysis.  
- Calculate key business metrics (KPIs) such as revenue, orders, and average order value.  
- Identify sales trends across days, hours, categories, and product sizes.  
- Determine the best-selling and least-selling calzones.  
- Provide actionable recommendations to improve sales performance.  

---
## Data Used
-<a href="https://github.com/ElizabethEboigbe/Calzone-Sales-Analysis-Excel/blob/main/Copy%20of%20calzone%20sales%20report.xlsx">Dataset</a>

## Dataset Description
 

The dataset contains order-level information, including:  
- Order ID  
- Product Name  
- Size  
- Quantity  
- Price  
- Order Date  
- Order Days  
- Unit Price  
- Product Size  
- Ingredients  
- Revenue  

 

---

## Data Cleaning & Preparation
 

- Removed duplicates: none were found.  
- Renamed products: changed “Pizza” to “Calzone.”  
- Standardized product sizes: used Find and Replace, changed “Regular” to “S”, “Medium” to “M”, “Large” to “L”, “XLarge” to “XL”, “XXLarge” to “XXL”.  
- Created new columns:  
  - **Distinct OrderID** using `=1/COUNTIF(B:B,[@[order_id]])`  
  - **Order Days** using `=TEXT(@F:F,"dddd")`  
- Checked for errors.  
- Formatted date column consistently.  

 

---

## KPIs Defined
 
- **Total Revenue** = Sum of all calzones ordered  
- **Total Calzones Sold** = Sum of all quantities  
- **Total Orders** = Distinct count of `order_id`  
- **Average Order Value (AOV)** = Total Revenue ÷ Total Orders  
- **Average Calzone per Order** = Total Calzones Sold ÷ Total Orders  

 
---

## Analysis & Visualizations
 
1. Daily Trend of Orders – Column Chart  
2. Hourly Trend of Orders – Line Chart  
3. % Sales by Category – Donut Chart  
4. % Sales by Size – 3D Pie Chart  
5. Total Calzones Sold by Category – Funnel Chart  
6. Top 5 Best-Selling Calzones – Bar Chart  
7. Bottom 5 Least-Selling Calzones – Bar Chart  
8. Interactive Dashboard combining all charts  

 

---

## Key Insights
 
- Sunday recorded the highest sales, while Wednesday recorded the lowest.  
- No sales data available for Thursday, Friday, and Saturday.  
- Classic category is the most popular, while Veggie category is the least popular.  
- Medium size is the most frequently ordered calzone.  

 
---

## Tools & Techniques Used
 

- **Excel** (Data Cleaning, Pivot Tables, KPIs, Visualizations, Dashboard)  
- **Formulas:** `COUNTIF`, `TEXT`, arithmetic calculations for KPIs  
- **Charts:** Column, Line, Donut, 3D Pie, Funnel, Bar  

 #3 Interactive dashboard
-<a href="https://github.com/ElizabethEboigbe/Calzone-Sales-Analysis-Excel/blob/main/Calzone%20Interactive%20Dashboard.xlsx">interactive dashboard</a>

---

## Recommendations
- **Boost Veggie Sales:** Increase marketing efforts (discounts, combos, campaigns) to attract more veggie calzone buyers.  
- **Leverage Peak Sales Day:** Employ more staff on Sundays and consider staff bonuses to handle high demand.  
- **Customer Feedback Loop:** Collect and analyze feedback to improve recipes and enhance customer satisfaction.  
- **Data Quality Check:** Investigate missing sales data for Thursday–Saturday to ensure accuracy.


<img width="1269" height="602" alt="calzone sales dashboard" src="https://github.com/user-attachments/assets/8d86def2-8ffb-46a8-8364-052bda032a05" />

