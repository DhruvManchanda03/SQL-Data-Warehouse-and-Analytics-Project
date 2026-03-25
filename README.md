# 📊 SQL Data Warehouse & Analytics Project

## 🚀 Project Overview

This project demonstrates the design and implementation of a **modern SQL-based data warehouse** using the **Medallion Architecture (Bronze → Silver → Gold)** approach.

The goal of this project is to:

* Ingest raw data from multiple sources (CRM & ERP)
* Clean and standardize the data
* Transform it into **business-ready datasets**
* Perform **analytical queries for insights**

---

## 🏗️ Architecture Overview

![Architecture](./assets/data_architecture.png)

The project follows a **layered Medallion Architecture**:

```
Sources → Bronze Layer → Silver Layer → Gold Layer → Analytics
```

---

## 🥉 Bronze Layer – Raw Data

### 📌 Purpose

The Bronze layer stores **raw, unprocessed data** exactly as received from source systems.

### ⚙️ Key Features

* Data loaded from **CSV files (CRM & ERP systems)**
* No transformations applied
* Preserves original data for traceability

### 🧱 Characteristics

* Object Type: Tables

* Data Model: None (as-is)

---

## 🥈 Silver Layer – Cleaned & Standardized Data

### 📌 Purpose

The Silver layer focuses on **data cleaning, validation, and standardization**.

### ⚙️ Transformations Performed

* Handling NULL and missing values
* Removing hidden characters (`\r`, `\n`, `\t`)
* Standardizing formats (dates, text, categories)
* Fixing inconsistent or invalid values
* Deriving new columns (e.g., corrected price, sales)
* Deduplication using window functions

### 🧱 Characteristics

* Object Type: Tables

* Data Model: Still normalized (not business-ready)

---

## 🥇 Gold Layer – Business Ready Data

### 📌 Purpose

The Gold layer provides **analytics-ready datasets** using a **star schema design**.

### ⭐ Data Model

* **Dimension Tables**

  * `dim_customers`
  * `dim_products`
* **Fact Table**

  * `fact_sales`

### ⚙️ Transformations

* Data integration across multiple sources
* Business logic implementation
* Aggregations and derived metrics
* Surrogate key generation

### 🧱 Characteristics

* Object Type: Views
* Data Model:

  * Star Schema
  * Optimized for analytics

---

## 📊 Analytics Performed

Using the Gold layer, several business insights were derived:

### 🔹 Sales Analysis

* Total sales by country
* Revenue distribution across product categories
* Top-performing products

### 🔹 Customer Insights

* Customer segmentation (e.g., single vs married)
* Number of unique customers purchasing specific product lines
* Age-based analysis

### 🔹 Order Insights

* Total number of orders per country
* Average order value (AOV)
* Order trends over time

---

## 🧠 Key Concepts Applied

* Medallion Architecture (Bronze, Silver, Gold)
* Data Cleaning & Standardization
* Window Functions
* Star Schema Modeling
* Fact & Dimension Design
* SQL Performance Optimization (Indexes, Joins)

---

## 🛠️ Tech Stack

* SQL (MySQL / SQL Server concepts)
* CSV Data Sources
* Stored Procedures
* Git & GitHub

---

## 📌 Key Learnings

* Designing a scalable data warehouse architecture
* Handling real-world dirty data issues
* Implementing business logic in SQL
* Writing optimized analytical queries

---

## 📈 Future Improvements

* Convert views into **materialized tables for performance**
* Add **indexes for faster query execution**
* Implement **incremental loading**
* Integrate with BI tools (Power BI / Tableau)

---

## 🙌 Acknowledgements

This project is inspired by real-world data engineering practices and aims to simulate an end-to-end data warehouse pipeline.

---

## ⭐ If you like this project

Give it a ⭐ on GitHub and feel free to connect!
