# E-commerce Customer Analysis

![Excel](https://img.shields.io/badge/Microsoft_Excel-Data_Analysis-217346)
![Google_Sheets](https://img.shields.io/badge/Google_Sheets-SQL_Queries-34A853)
![Statistics](https://img.shields.io/badge/Statistics-Correlation_Analysis-orange)
![Regression](https://img.shields.io/badge/Model-Linear_Regression-green)
![SQL](https://img.shields.io/badge/SQL-Data_Exploration-blue)
![Business_Intelligence](https://img.shields.io/badge/Business-Insights-blueviolet)

---

##  Project Overview 
E-commerce customer behavior analysis covering data cleaning, statistical modeling, 
and SQL exploration in spreadsheets. Identified peak sales patterns and market 
concentration for business optimization.

---

## Key Insights:
- 95% revenue concentration in UK market
- Peak sales hours: 11 AM - 12 PM  
- Weak negative price-quantity correlation
- Top product: "Assorted Colour Bird Ornament"
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

Sales Visualization <img width="867" height="526" alt="image" src="https://github.com/user-attachments/assets/77f814d5-2be2-4bb3-88a3-303b54008330" />

---

### **5. Model Data (Linear Regression)**  
**Objective:** Examine the price–quantity relationship to understand demand patterns.  

**Regression Formula:**
Price = -0.0029 × Quantity + 3.31

**Interpretation:**  
Indicates a **weak negative correlation**, supporting the **demand curve principle** — higher quantity tends to associate with slightly lower prices.

---

## Key Business Insights

### Strengths
- **95% UK Market Dominance** - Strong home market presence
- **Clear Peak Hours** - 11 AM-12 PM for targeted marketing
- **Product Leadership** - Home & kitchen categories driving revenue

### Growth Opportunities  
- **International Expansion** - France & Germany markets
- **Time-Based Promotions** - Capitalize on peak sales hours
- **Customer Segmentation** - Domestic vs international strategies

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

### Data Pipeline
1. **Data Cleaning** - Remove duplicates, filter invalid transactions
2. **Feature Engineering** - Revenue calculations, time binning
3. **Statistical Analysis** - Correlation, regression modeling
4. **SQL Exploration** - Google Sheets QUERY function
5. **Visualization** - Pivot charts, trend analysis

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
