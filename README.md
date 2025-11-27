# E-commerce Customer Analysis
![Excel](https://img.shields.io/badge/Microsoft_Excel-Data_Analysis-217346)
![Google_Sheets](https://img.shields.io/badge/Google_Sheets-SQL_Queries-34A853)
![Statistics](https://img.shields.io/badge/Statistics-Correlation_Analysis-orange)
![Regression](https://img.shields.io/badge/Model-Linear_Regression-green)
![SQL](https://img.shields.io/badge/SQL-Data_Exploration-blue)
![Business_Intelligence](https://img.shields.io/badge/Business-Insights-blueviolet)

---

## Project Overview
Analysis of **E-commerce customer behavior** using Excel and Google Sheets with SQL-like queries.  
Focused on **data cleaning, statistical modeling, visual insights, and revenue optimization**.

**Dataset:** Transactions including Invoice, Product, Quantity, Price, Customer, Country  

---

## Key Insights
- **Revenue Concentration:** 95% from UK market  
- **Peak Sales Hour:** 11 AM – 12 PM  
- **Top Product:** "Assorted Colour Bird Ornament" (~\$1,160 revenue)  
- **Price-Quantity Relationship:** Weak negative correlation (-0.139)  

---

## Data Cleaning & Preparation
**Operations:**
- Removed duplicates, cancelled orders, postage/refund transactions  
- Converted Excel date serials to readable datetime  
- Created calculated columns: **Revenue**, **Time (hour bins)**  

**Outcome:** Clean, analysis-ready dataset for insights and modeling  

---


## Sales Visualization
<img width="867" height="526" alt="Peak Hour Sales Analysis" src="https://github.com/user-attachments/assets/77f814d5-2be2-4bb3-88a3-303b54008330" />

*Peak sales hours and geographic revenue distribution*



## Statistical & Visual Analysis
| Metric | Value | Insight |
|--------|-------|---------|
| Total Revenue | \$116.85 | From clean transactions |
| Avg Price | \$3.20 | Consistent pricing |
| Price Range | \$0.55 – \$12.75 | Product diversity |

**Peak Hours & Market:**
- **Hour:** 11 AM – 12 PM  
- **Market Share:** 87% UK, 13% international

---

## Regression Analysis
**Objective:** Examine Price → Quantity relationship  
**Formula:** Price = -0.0029 × Quantity + 3.31  
**Interpretation:** Weak negative correlation confirms slight price drop at higher quantities

---

## Business Insights & Recommendations
**Strengths**
- Dominant UK market (95% revenue)  
- Clear peak hours for targeted campaigns  
- High-performing products in home décor & kitchen  

**Opportunities**
- Expand into France & Germany markets  
- Time-based promotions during peak hours  
- Customer segmentation strategies (Domestic vs International)  

---

## SQL Exploration in Google Sheets
Used **QUERY function** to analyze patterns:  
- `SELECT` & `WHERE` → Filter by product, country, or date  
- `GROUP BY` → Aggregate revenue by country/product  
- `ORDER BY` & `LIMIT` → Top-performing products  
- Aggregations: `SUM()`, `AVG()`, `MAX()`, `MIN()`  

**[View SQL Queries →](https://docs.google.com/spreadsheets/d/18q1ex-GEzD1l5qjpdhAf7B6X1F7EaQyAJ4ZtaEzPN5A/edit?usp=sharing)**

---

## Technical Implementation
1. **Data Cleaning** – Remove duplicates, cancelled orders, invalid transactions  
2. **Feature Engineering** – Revenue calculation, time binning  
3. **Statistical Analysis** – Correlation & regression modeling  
4. **SQL Exploration** – Google Sheets QUERY for insights  
5. **Visualization** – Pivot tables, charts, and peak-hour trends  

---

## Files Included
- `1_Cleaning_&_Exploring.xlsx` – Full Excel analysis workflow  
- `2_Extracting_Data_with_SQL` – Google Sheets SQL queries  

---

## Tools & Skills
- **Excel:** Cleaning, Pivot Tables, Charts, Descriptive Stats  
- **Google Sheets:** SQL-like queries (QUERY function)  
- **Stats & Modeling:** Correlation, Linear Regression  
- **Visualization:** Aggregation charts, trend plots  

---

## Project Context
**Course:** Data Analysis with Spreadsheets & SQL  
**Program:** Meta Data Analyst with GenAI Professional Certificate  
**Objective:** Apply spreadsheet analytics & SQL techniques to deliver actionable business insights
