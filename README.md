# E-commerce Customer Analysis

![Excel](https://img.shields.io/badge/Microsoft_Excel-Data_Analysis-217346)
![Google_Sheets](https://img.shields.io/badge/Google_Sheets-SQL_Queries-34A853)
![Statistics](https://img.shields.io/badge/Statistics-Correlation_Analysis-orange)
![Regression](https://img.shields.io/badge/Model-Linear_Regression-green)
![SQL](https://img.shields.io/badge/SQL-Data_Exploration-blue)
![Business_Intelligence](https://img.shields.io/badge/Business-Insights-blueviolet)

---

##  Project Overview  
This project demonstrates a **comprehensive data analysis workflow** on e-commerce transaction data, covering the **entire analytics pipeline** — from data cleaning to statistical analysis, visualization, predictive modeling, and SQL-based exploration in **Google Sheets**.  

The goal was to uncover actionable insights into **customer purchasing behavior**, **sales trends**, and **market opportunities**.

---

##  Excel Workbook Breakdown  

### **1. Customer Data (Raw)**  
**Purpose:** Initial dataset containing unprocessed transactional data.  
**Key Columns:** Invoice, StockCode, Description, Quantity, InvoiceDate, Price, Customer ID, Country  

**Data Issues Identified:**
- Duplicate records  
- Cancelled orders (Invoices with ‘C’ prefix)  
- Missing customer IDs and descriptions  
- Postage/refund transactions  
- Unformatted Excel date serials  

---

### **2. Clean Data**  
**Purpose:** Transformed dataset ready for analysis.  

**Cleaning Operations:**
- Removed duplicates and cancelled orders  
- Filtered out postage, refunds, and zero-value transactions  
- Converted Excel date serials → readable datetime  
- Created calculated columns: **Revenue** and **Time (hour bins)**  

**Final Dataset:** 45 valid transactions  

---

### **3. Exploring Data Numerically**  
**Purpose:** Statistical exploration and relationship analysis.  

| Metric | Value | Insight |
|--------|--------|----------|
| **Total Price** | \$116.85 | Total revenue from clean transactions |
| **Average Price** | \$3.20 | Average item cost |
| **Median Price** | \$2.60 | Consistent price distribution |
| **Price Range** | \$0.55 – \$12.75 | Healthy product diversity |

**Correlation Analysis:**
- Price ↔ Quantity: **-0.139** (weak negative relationship)  
- Invoice Date ↔ Price: **0.108** (very weak positive relationship)

---

### **4. Exploring Data Visually**  
**Purpose:** Visual analysis using Excel pivot charts and aggregated summaries.  

**Key Insights:**
- **Peak Hour:** 11 AM – 12 PM (highest daily sales)  
- **Top Market:** United Kingdom (≈95% revenue share)  
- **Top Product:** “ASSORTED COLOUR BIRD ORNAMENT” (~\$1,160 revenue)  
- **Customer Distribution:** 87% UK-based, 13% international  

Visuals <img width="867" height="526" alt="image" src="https://github.com/user-attachments/assets/77f814d5-2be2-4bb3-88a3-303b54008330" />

---

### **5. Model Data (Linear Regression)**  
**Objective:** Examine the price–quantity relationship to understand demand patterns.  

**Regression Formula:**
Price = -0.0029 × Quantity + 3.31

**Interpretation:**  
Indicates a **weak negative correlation**, supporting the **demand curve principle** — higher quantity tends to associate with slightly lower prices.

---

## Key Business Insights  

### **Strengths**
- Strong UK market presence and consistent customer engagement  
- Clear **peak-hour sales patterns** for operational optimization  
- High-performing **home & kitchen categories**  
- Well-defined customer purchasing trends  

### **Opportunities**
- **Geographic Expansion:** Grow presence in France, Germany, and other European markets  
- **Time-Based Marketing:** Focus promotions during **11 AM – 12 PM** peak window  
- **Product Diversification:** Expand top-performing categories  
- **Customer Segmentation:** Tailor offers for **domestic vs international** audiences  

---

## SQL Queries (in Google Sheets)

Executed SQL-like queries using **Google Sheets QUERY function** for data exploration:

| Query Type | Purpose |
|-------------|----------|
| `SELECT ... WHERE` | Filter transactions by product, country, or date |
| `ORDER BY` & `LIMIT` | Sort and extract top-performing products |
| `GROUP BY` | Aggregate sales by country or product |
| `AVG()`, `SUM()`, `MAX()`, `MIN()` | Calculate key performance metrics |
| Conditional expressions | Analyze filtered patterns and KPIs |

**[View Google Sheets SQL Workbook →](https://docs.google.com/spreadsheets/d/18q1ex-GEzD1l5qjpdhAf7B6X1F7EaQyAJ4ZtaEzPN5A/edit?usp=sharing)**

---

## Technical Implementation  

### **Data Cleaning Steps**
- Removed duplicates and invalid transactions  
- Filtered cancellations, refunds, and postage charges  
- Converted dates and engineered new columns (Revenue, Time)  

### **Analytical Techniques**
- **Descriptive Statistics:** Mean, median, and spread metrics  
- **Correlation Analysis:** Numerical relationship exploration  
- **Visual Analytics:** Pivot charts and sales distribution plots  
- **Predictive Modeling:** Linear regression for price–quantity dynamics  

---

## Recommendations

1. **Expand International Markets:** Target France and Germany for regional growth  
2. **Leverage Peak Hours:** Optimize ads and discounts between **11 AM – 12 PM**  
3. **Product Strategy:** Double down on high-margin home décor and kitchen products  
4. **Customer Segmentation:** Develop tailored retention programs for domestic vs international clients  

---

## Files Included

- [1_Cleaning_&_Exploring.xlsx](1_Cleaning_&_Exploring.xlsx) — Main Excel workbook with the full analysis pipeline
- [2_Extracting_Data_with_SQL](2_Extracting_Data_with_SQL) — Google Sheets SQL queries


## Tools & Techniques  

- **Microsoft Excel:** Data Cleaning • Pivot Tables • Charts • Descriptive Stats  
- **Google Sheets:** SQL-like Queries (QUERY function)  
- **Statistical Methods:** Correlation • Regression • Hypothesis-based Analysis  
- **Visualization:** Aggregation charts • Peak-hour sales trend plots
---

## Project Context  

**Course:** Data Analysis with Spreadsheets and SQL  
**Program:** Meta Data Analyst with GenAI Professional Certificate  
**Focus:** Applying spreadsheet-based analytics and SQL techniques for business intelligence  
