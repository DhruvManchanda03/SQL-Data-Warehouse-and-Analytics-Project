## 📊 Dashboard & Visualization Layer

The dashboard layer is built on top of the **Gold Layer** of the data warehouse, ensuring all visualizations are powered by **clean, business-ready, and aggregated data**.

The dashboards provide interactive insights across **sales, customers, and products**, enabling data-driven decision-making.

---

## 🔌 Data Source

All dashboards are directly connected to:

- Gold Layer tables (`fact_sales`, `dim_customers`, `dim_products`, etc.)
- Aggregated views (`report_customers`, `report_products`)

This ensures:
- High performance ⚡
- Consistent business logic ✅
- Scalable reporting 📈

---

## 📈 Dashboard Pages

### 1. Executive Overview
- High-level KPIs:
  - Revenue
  - Total Orders
  - Units Sold
  - Customers
  - Average Order Value
- Sales trend over time
- Revenue breakdown by category and country

---

### 2. Sales Analysis
- Monthly sales trends
- Top-performing products
- Revenue distribution by category
- Year-based filtering

---

### 3. Product Analysis
- Revenue by product category & segment
- Top 5 products by revenue
- Units sold by category
- Category & subcategory filters

---

### 4. Customer Analysis
- Customer distribution (gender, age)
- Customers by country
- Top customers by revenue
- Customer segmentation (VIP, Regular, New)

---

## 🎯 Key Features

- Interactive filters (Year, Country, Category)
- Drill-down capabilities
- Dynamic KPI tracking
- Clean and intuitive UI design

---

## 🛠️ Tools Used

- Power BI (for dashboard development)
- SQL (Gold Layer as data source)

---

## 📌 Purpose

The dashboard layer transforms structured warehouse data into:
- Actionable insights
- Business intelligence reports
- Executive-level summaries

It serves as the final layer of the data pipeline, bridging **data engineering → analytics → decision-making**.

---
