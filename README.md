# 📊 Retail Sales Analytics Dashboard — Excel

> **Project #1 · Excel · Data Cleaning · Pivot Tables · Dashboard Design**

---

## 🗂️ Project Overview

A **6-month retail sales analysis** built entirely in Microsoft Excel, covering revenue performance, salesperson metrics, category breakdowns, and regional trends. The raw dataset was intentionally embedded with real-world data quality issues — duplicates, flagged records, and returns — to simulate a production data environment.

This project demonstrates the fundamentals of the data analyst workflow: **ingest → audit → clean → analyse → visualise.**

---

## 📁 File Structure

```
retail-sales-excel-dashboard/
│
├── retail_sales_6_months.xlsx       # Main workbook
│   ├── raw_data                     # Source data with embedded quality issues
│   ├── cleaned_data                 # Post-audit, validated dataset
│   ├── pivot_analysis               # Pivot tables for KPIs
│   └── dashboard                   # Final visual dashboard
│
└── README.md
```

---

## 🧩 Dataset Details

| Attribute | Detail |
|---|---|
| **Period** | 6 Months (2026) |
| **Rows** | ~1,050 transactions |
| **Products** | Laptop, Mobile, Monitor, Headphones, Printer, Chair, Table |
| **Categories** | Electronics, Furniture |
| **Regions** | North, East, West, South |
| **Salespersons** | Meena, Karthik, Priya, Ravi, Arjun, Sneha |
| **Transaction Types** | Sale, Return |

### 🚩 Embedded Data Quality Issues (by design)

| Issue Type | Count | Description |
|---|---|---|
| **Duplicates** | 82 | Duplicate order entries |
| **Flagged Rows** | 111 | Missing Revenue or Cost values |
| **Returns** | 27 | Negative revenue transactions |
| **Remove** | 2 | Invalid / corrupt records |

---

## 🔍 Analysis Performed

### 1. Data Audit & Cleaning
- Identified and flagged 111 records with missing Revenue or Cost
- Isolated 82 duplicate rows using conditional formatting + COUNTIF
- Separated returns (27 rows) from gross sales for accurate KPI reporting
- Final clean dataset: **968 valid unique sale transactions**

### 2. Key KPIs (Pivot Tables)
- **Total Revenue** | **Total Units Sold** | **Total Profit**
- **Profit Margin %** by Category and Region
- **Month-over-Month Revenue** trend (Jan–Dec 2026)
- **Top Salesperson** by Revenue and by Units Sold

### 3. Category & Product Performance
- Electronics vs Furniture revenue split
- Product-level revenue ranking (Laptop, Monitor leading)
- Return rate by category

### 4. Regional Analysis
- Revenue contribution % by region (North / East / West / South)
- Salesperson-to-region mapping
- Best-performing region by profit margin

### 5. Dashboard
- Single-page interactive dashboard with slicers (Region, Category, Month)
- Dynamic charts: Bar chart (monthly revenue), Donut (category split), Column (salesperson comparison)

---

## 💡 Key Findings

- **Electronics** dominates revenue, contributing ~65–70% of total sales
- **Meena** is the highest-revenue salesperson across most months
- **Flagged rows (111)** represented a significant data quality risk — if uncleaned, gross revenue figures would be materially misstated
- **Return rate** was low (~2.5%) suggesting healthy transaction quality once duplicates are removed

---

## 🛠️ Tools & Techniques

| Tool / Feature | Used For |
|---|---|
| **Excel Pivot Tables** | KPI aggregations, cross-tab analysis |
| **COUNTIF / IF / IFERROR** | Duplicate detection, conditional flags |
| **Conditional Formatting** | Highlighting anomalies in raw data |
| **Slicers** | Interactive dashboard filtering |
| **Charts** | Bar, Column, Donut, Line |
| **Data Validation** | Clean data integrity checks |

---

## 🎯 Skills Demonstrated

- Real-world **data auditing** and cleaning workflow
- Designing for **data quality** (not just analysis)
- **Pivot table** mastery with calculated fields
- Dashboard design within **Excel constraints**
- Business storytelling through **visual layout**

---

## 📌 Notes

This is **Portfolio Project #1** in a progressive analytics portfolio:

| # | Project | Stack |
|---|---|---|
| 1 | **Retail Sales Dashboard** ← You are here | Excel |
| 2 | ShopSphere Sales Analysis | SQL + Power BI |
| 3 | A-OEM Enterprise Analytics Ecosystem | PostgreSQL · Python · Power BI |

---

*Built as part of a data analytics portfolio. Dataset is synthetic.*
