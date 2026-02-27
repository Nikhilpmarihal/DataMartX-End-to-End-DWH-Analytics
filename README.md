![DWH SQL drawio](https://github.com/user-attachments/assets/8fd70213-8e2b-4140-8702-f91b0d142cd6)


# 📊 SQL Server Data Warehouse & Analytics Project

## 🚀 Overview

This project demonstrates the end-to-end design and implementation of a **modern data warehouse solution using SQL Server**, including ETL processes, dimensional data modeling, and SQL-based analytics.

The objective is to consolidate sales data from multiple source systems into a unified analytical model that supports reporting, business intelligence, and strategic decision-making.

This repository reflects industry best practices in:

* Data Engineering
* Data Modeling
* Data Quality Management
* Analytical SQL Development
* Business Intelligence Reporting

---

## 🏗️ Project Architecture

The solution follows a structured data warehousing pipeline:

1. **Data Ingestion** – Import raw CSV files from ERP and CRM systems
2. **Data Cleansing** – Resolve inconsistencies, nulls, duplicates, and formatting issues
3. **Data Integration** – Merge datasets into a unified schema
4. **Dimensional Modeling** – Create fact and dimension tables optimized for analytics
5. **Analytics Layer** – Develop SQL queries to generate business insights

---

## 🎯 Project Objectives

### 1️⃣ Data Engineering – Build the Data Warehouse

**Goal:**
Develop a centralized SQL Server data warehouse to consolidate sales data for analytical reporting.

### Specifications

* **Data Sources**

  * ERP system (CSV files)
  * CRM system (CSV files)

* **Data Quality Management**

  * Handle missing values
  * Remove duplicates
  * Standardize data formats
  * Validate referential integrity

* **Data Integration**

  * Combine ERP and CRM datasets
  * Create a unified, analytics-friendly schema

* **Scope**

  * Focus on the latest dataset
  * No historization (no SCD implementation)

* **Documentation**

  * Provide clear schema documentation
  * Ensure stakeholder-friendly structure

---

### 2️⃣ Data Analytics – Business Intelligence with SQL

**Goal:**
Develop SQL-based analytics to generate actionable business insights.

### Key Analytical Areas

* 👥 Customer Behavior

  * Customer segmentation
  * Repeat purchase patterns
  * Revenue contribution per customer

* 📦 Product Performance

  * Best-selling products
  * Revenue by product category
  * Product profitability analysis

* 📈 Sales Trends

  * Monthly sales performance
  * Revenue growth analysis
  * Seasonal trends

These insights enable data-driven decision-making for business stakeholders.

---

## 🗄️ Data Model Design

The warehouse follows a **Dimensional Modeling (Star Schema)** approach.

### Core Components

**Fact Table**

* `FactSales`

  * Sales Amount
  * Quantity
  * Transaction Date
  * Customer Key
  * Product Key

**Dimension Tables**

* `DimCustomer`
* `DimProduct`
* `DimDate`
* (Optional additional dimensions as required)

This design ensures:

* Optimized query performance
* Simplified analytical queries
* Scalability for future expansion

---

## 🔄 ETL Process

The ETL pipeline includes:

1. **Extract**

   * Import CSV files into staging tables

2. **Transform**

   * Clean and standardize data
   * Apply transformations
   * Map business keys to surrogate keys

3. **Load**

   * Load cleaned data into fact and dimension tables

All transformations are implemented using **SQL Server scripts**.

---

## 📊 Sample Analytics Queries

Examples of insights generated:

* Total Revenue by Month
* Top 10 Customers by Revenue
* Top Performing Products
* Sales Growth Percentage
* Revenue by Customer Segment









