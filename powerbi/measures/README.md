# DAX Measures & Metric Logic

This folder documents the key DAX measures used across the Power BI reports.

The measures were designed to ensure **metric consistency**, enable **time‑intelligence analysis**, and support **reliable business insights** across all dashboards.

Rather than listing every formula, this section describes the **measure structure, categories, and analytical intent**.

---

## 🧩 Measure Design Principles

- Separation of base measures and derived metrics
- Centralized measure table for clarity and governance
- Reusable logic to avoid duplication
- Explicit handling of missing or invalid data
- Alignment with dimensional star schema modeling

---

## 📊 Core Business Measures

These measures establish the foundation for performance analysis:

- **Total Sales**
- **Total Quantity Sold**
- **Total Orders**
- **Total Completed Orders**
- **Gross Cost**
- **Gross Margin**
- **Gross Margin Percentage**

These KPIs are used across all performance and profitability dashboards.

---

## ⏱ Time‑Intelligence Measures

Time‑based measures were created using the dedicated Date dimension to support trend and comparison analysis:

- Year‑to‑Date (YTD)
- Month‑to‑Date (MTD)
- Quarter‑to‑Date (QTD)
- Prior Year (PY) comparisons
- Year‑over‑Year (YoY) growth

These measures allow consistent temporal comparisons across all visuals.

---

## 👥 Customer & Value Metrics

To analyze customer behavior and value contribution, the following measures were developed:

- Average Order Value (AOV)
- Customer Retention Rate
- New vs Repeat Customers
- Customer Lifetime Value (CLV)
- Repeat Purchase Rate

These metrics shift analysis from **vanity metrics** (sales volume) to **value metrics** (profitability per customer).

---

## 🧪 Diagnostic & Data‑Quality Measures

Additional measures were created to monitor data integrity and analytical reliability:

- Orders with Missing Customer
- Orders with Missing Store
- Orders with Missing Unit Price
- Negative Shipping Delay Flags

These diagnostics ensure insights are based on trustworthy data.

---

## 🔀 Dynamic & Advanced Measures

To support deeper analysis, several advanced techniques were implemented:

- Dynamic X/Y selector measures for correlation analysis
- Measure selector tables (disconnected)
- Median, minimum, and maximum sales measures
- Discount and unit price analysis metrics

These measures enable flexible exploration without duplicating logic.

---

## ✅ Summary

The DAX measures in this project were designed to support:
- Consistent analytics across dashboards
- Scalable report development
- Transparent metric definitions
- Business‑focused interpretation, not just calculations

They form the analytical backbone of the Power BI reports.
