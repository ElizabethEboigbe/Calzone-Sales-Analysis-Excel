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

## Dataset Description
<details>
<summary>Click to expand</summary>

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

</details>

---

## Data Cleaning & Preparation
<details>
<summary>Click to expand</summary>

- Removed duplicates: none were found.  
- Renamed products: changed “Pizza” to “Calzone.”  
- Standardized product sizes: used Find and Replace, changed “Regular” to “S”, “Medium” to “M”, “Large” to “L”, “XLarge” to “XL”, “XXLarge” to “XXL”.  
- Created new columns:  
  - **Distinct OrderID** using `=1/COUNTIF(B:B,[@[order_id]])`  
  - **Order Days** using `=TEXT(@F:F,"dddd")`  
- Checked for errors.  
- Formatted date column consistently.  

</details>

---

## KPIs Defined
<details>
<summary>Click to expand</summary>

- **Total Revenue** = Sum of all calzones ordered  
- **Total Calzones Sold** = Sum of all quantities  
- **Total Orders** = Distinct count of `order_id`  
- **Average Order Value (AOV)** = Total Revenue ÷ Total Orders  
- **Average Calzone per Order** = Total Calzones Sold ÷ Total Orders  

</details>

---

## Analysis & Visualizations
<details>
<summary>Click to expand</summary>

1. Daily Trend of Orders – Column Chart  
2. Hourly Trend of Orders – Line Chart  
3. % Sales by Category – Donut Chart  
4. % Sales by Size – 3D Pie Chart  
5. Total Calzones Sold by Category – Funnel Chart  
6. Top 5 Best-Selling Calzones – Bar Chart  
7. Bottom 5 Least-Selling Calzones – Bar Chart  
8. Interactive Dashboard combining all charts  

</details>

---

## Key Insights
<details>
<summary>Click to expand</summary>

- Sunday recorded the highest sales, while Wednesday recorded the lowest.  
- No sales data available for Thursday, Friday, and Saturday.  
- Classic category is the most popular, while Veggie category is the least popular.  
- Medium size is the most frequently ordered calzone.  

</details>

---

## Tools & Techniques Used
<details>
<summary>Click to expand</summary>

- **Excel** (Data Cleaning, Pivot Tables, KPIs, Visualizations, Dashboard)  
- **Formulas:** `COUNTIF`, `TEXT`, arithmetic calculations for KPIs  
- **Charts:** Column, Line, Donut, 3D Pie, Funnel, Bar  

</details>

---

## Recommendations
- **Boost Veggie Sales:** Increase marketing efforts (discounts, combos, campaigns) to attract more veggie calzone buyers.  
- **Leverage Peak Sales Day:** Employ more staff on Sundays and consider staff bonuses to handle high demand.  
- **Customer Feedback Loop:** Collect and analyze feedback to improve recipes and enhance customer satisfaction.  
- **Data Quality Check:** Investigate missing sales data for Thursday–Saturday to ensure accuracy.  
