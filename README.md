# 🛍️ Retail Clothing Data Analytics
**End‑to‑End Data Wrangling, Dimensional Modeling & Business Intelligence**

---

## 📌 Project Overview

This repository presents an **end‑to‑end retail data analytics project** that transforms raw transactional data into **business‑ready insights** using structured data preparation, dimensional modeling, and Power BI reporting.

Rather than focusing solely on dashboard visuals, this project emphasizes:
- **Data quality and reliability**
- **Analytical feature engineering**
- **Robust data modeling (Star Schema)**
- **Validated metrics and time‑intelligence**
- **Insight‑driven decision support**

The work demonstrates how disciplined data preparation and modeling enable trustworthy analytics and meaningful business conclusions.

---

## 🎯 Business Problem Statement

Initial exploratory analysis revealed a critical issue:

> **Sales volume was increasing significantly, but overall profitability was declining.**

This raised several business questions:
- Are margin declines driven by product mix, pricing decisions, or rising costs?
- Do higher sales volumes translate into higher customer value?
- Is business growth driven by customer retention or constant acquisition?
- Which channels, categories, and customers truly generate profit?

This project was designed to answer those questions using data.

---

## 🧹 Data Preparation & Wrangling (Power Query)

A **structured and auditable data‑wrangling process** was implemented using **Power Query** in Power BI.

### Key Data Engineering Steps
- Verified and standardized data types across all tables
- Cleaned and normalized text fields (trim, clean, capitalization)
- Consolidated customer identity fields to reduce duplication
- Engineered analytical features:
  - Customer age calculation
  - Email availability indicators
  - Product price band segmentation
  - Shipping delay metrics
  - Transaction‑level revenue (`LineAmount`)
- Flagged anomalies such as negative shipping delays
- Implemented data‑quality checks for missing customer, store, and pricing values

All transformation steps were documented in a **step‑by‑step wrangling log** to ensure transparency and reproducibility.

📂 Detailed transformation logic is stored in the `data-wrangling/` directory.

---

## 🧱 Data Modeling & Architecture

A **dimensional Star Schema** was implemented to support scalable analytics and reliable DAX calculations.

### Model Design
- **Fact table:** Sales transactions  
- **Dimension tables:** Customer, Product, Store, Date  

### Modeling Principles
- One‑to‑many relationships from dimensions to the fact table
- Removal of auto‑generated Power BI relationships
- Dedicated Date table created using DAX for time‑intelligence
- Centralized measure table for calculation governance

### Benefits
- Accurate aggregations and filtering
- Improved Power BI performance
- Reliable year‑over‑year and period‑based analysis
- Clear separation of facts and dimensions

---

## 📐 Measures & Analytics (DAX)

The project goes beyond basic KPIs by implementing **diagnostic and advanced measures**.

### Core Business Measures
- Total Sales
- Total Quantity
- Orders / Completed Orders
- Gross Cost
- Gross Margin and Margin %

### Time‑Intelligence Measures
- Year‑to‑Date (YTD)
- Month‑to‑Date (MTD)
- Quarter‑to‑Date (QTD)
- Prior‑Year and Year‑over‑Year comparisons
- Shipped vs Ordered sales analysis

### Advanced & Diagnostic Measures
- Data‑quality metrics for missing keys
- Average Order Value (AOV)
- Average Unit Price
- Discount impact analysis
- Dynamic X/Y measures for correlation analysis
- Customer metrics:
  - New vs Repeat Customers
  - Customer Retention Rate
  - Customer Lifetime Value (CLV)
  - RFM‑based segmentation

All DAX measures were centrally organized to ensure consistency and maintainability.

---

## 📊 Key Insights & Findings

The analysis revealed several important patterns:

- **Strong sales growth masked declining profitability**
- Margin erosion was driven primarily by **low‑margin product categories**
- A small number of categories contributed disproportionately to overall profit
- Growth was **acquisition‑led**, not driven by customer loyalty
- Customer retention and repeat purchase rates were weak
- Higher‑value transactions were concentrated in specific sales channels
- Data completeness issues directly affected segmentation accuracy

These insights shifted the narrative from surface‑level sales performance to **value efficiency and long‑term sustainability**.

---

## 💡 Data‑Driven Recommendations

Based on the findings, several strategic recommendations were proposed:
- Transition from a **volume‑first** to a **value‑based** growth strategy
- Prioritize high‑margin product categories
- Improve customer retention through post‑purchase engagement
- Optimize pricing and discount strategies
- Focus channel investment on higher AOV performance
- Address data‑quality gaps to improve decision confidence

All recommendations are grounded in quantified metrics rather than assumptions.

---

## 🛠 Tools & Technologies Used

- **Power BI**
  - Power Query (Data Transformation)
  - DAX (Measures & Time Intelligence)
  - Data Modeling (Star Schema)
- **Microsoft Excel**
  - Data wrangling and transformation audit logs
- **Retail transactional datasets**
- **Dimensional modeling best practices**

---

## 👤 Individual Contribution

This project was completed as part of a group assignment.

**My individual contributions focused on:**
- Data‑wrangling strategy and transformation logic
- Power Query implementation and feature engineering
- Data‑quality validation and anomaly detection
- Star schema design and relationship modeling
- DAX measure development and time‑intelligence calculations
- Interpretation and synthesis of analytical insights

---

## 📁 Repository Structure

```
retail-clothing-data-analytics/
├── README.md
├── data-wrangling/
│   └── GroupBMW_Part1_Log.xlsx
├── powerbi/
│   ├── model/
│   ├── dashboards/
│   └── measures/
├── insights/
└── documentation/
```

## ⚠️ Disclaimer

This project was developed for **academic and portfolio demonstration purposes**.  
The dataset and insights are used to illustrate data analytics and BI techniques and are not intended for real‑world deployment.
