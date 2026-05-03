# Amazon-Sales-Report

A full end-to-end data analysis project on Amazon India sales data
using Python and SQL.

---

## 📌 Project Overview

| Detail | Info |
|---|---|
| Dataset | Amazon India Sales Report |
| Time Period | April 2022 – June 2022 |
| Raw Rows | 1,28,975 |
| Clean Rows | 1,21,177 |
| Tools Used | Python, Pandas, Seaborn, Matplotlib, SQLite |

---

## ⚙️ Steps Performed

### Step 1 — Data Cleaning
- Dropped junk columns (`Unnamed: 22`, `index`)
- Standardised all column names to `lowercase_underscore`
- Converted `Date` from string to datetime
- Converted `Amount` and `Qty` to numeric types
- Dropped rows with missing `Amount` or `Date` (7,798 rows)
- Removed 3 duplicate rows
- Standardised state names to UPPERCASE
- Created 3 new columns: `revenue`, `month`, `week`

### Step 2 — Exploratory Data Analysis
- Analysed revenue by category, state, size, fulfilment
- Identified cancellation rate and delivery status
- Compared B2B vs B2C segments
- Plotted 10 charts using Seaborn and Matplotlib

### Step 3 — SQL Analysis
- Loaded cleaned data into SQLite database
- Wrote 15 SQL queries using SELECT, GROUP BY,
  WHERE, HAVING, ORDER BY, LIMIT, window functions

---

## 📊 Charts

### Revenue by Category
![Revenue by Category](charts/chart1_revenue_by_category.png)

### Monthly Revenue Trend
![Monthly Trend](charts/chart2_monthly_trend.png)

### Order Status Distribution
![Order Status](charts/chart3_order_status.png)

### Top 10 States by Revenue
![Top States](charts/chart4_top_states.png)

### Orders by Size
![Size Distribution](charts/chart5_size_distribution.png)

### Order Amount Distribution
![Amount Distribution](charts/chart6_amount_distribution.png)

### Revenue Heatmap — Category vs Size
![Heatmap](charts/chart7_heatmap_cat_size.png)

### Revenue by Fulfilment Type
![Fulfilment](charts/chart8_fulfilment.png)

### Boxplot — Amount by Category
![Boxplot](charts/chart9_boxplot_category.png)

### Correlation Heatmap
![Correlation](charts/chart10_correlation.png)

---

## 🔑 Key Business Insights

1. **Set** is the #1 category — ₹3.79 Cr revenue, ₹833 avg order value
2. **Maharashtra & Karnataka** = 37% of total revenue
3. **8.9% cancellation rate** = ₹96 lakh lost revenue
4. **64% orders** still show Shipped — delivery tracking lag
5. **Size M & L** are most popular — never let these go out of stock
6. **B2B avg order = ₹55,000** vs B2C ₹627 — huge B2B opportunity
7. **May 2022** was peak month — stock up before April every year
8. **Amazon Fulfilled** handles 70% orders vs 30% Merchant
9. **Set category** has highest cancellations — needs investigation
10. **Premium orders (₹1000+)** are mostly Set & Western Dress

