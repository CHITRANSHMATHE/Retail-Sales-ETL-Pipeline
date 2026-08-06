# Retail-Sales-ETL-Pipeline using PySpark
An end-to-end ETL pipeline that ingests raw retail transaction data, performs automated data quality checks, transforms records, exports them into multiple formats (CSV, JSON, Parquet), and loads the cleaned data into MySQL for analytics.

## Project Overview

This project demonstrates an end-to-end ETL (Extract, Transform, Load) pipeline built using PySpark to process retail sales data. The pipeline performs data ingestion, profiling, cleaning, transformation, feature engineering, and Spark SQL analytics to generate business insights from raw transactional data.

The project follows a modular ETL workflow commonly used in modern data engineering pipelines.

---

## Problem Statement

Retail organizations generate large volumes of transactional data that often contain inconsistencies such as duplicate records, missing values, inconsistent formatting, and invalid data types. This project focuses on building a scalable ETL pipeline to clean, transform, and prepare retail sales data for downstream analytical reporting.

---

## Dataset

- Retail Sales Dataset
- Records : 9,994+
- Format : CSV

---

## Technologies Used

- PySpark
- Python
- Spark SQL
- Jupyter Notebook
- Git & GitHub

---

## ETL Workflow

Extract

- Read raw CSV data
- Inspect schema
- Profile dataset

Transform

- Standardize column names
- Handle missing values
- Remove duplicate records
- Validate data quality
- Feature engineering
- Business rule validation

Load

- Spark SQL Analysis
- Export Layer (CSV / JSON / Parquet) *(Pending Windows Hadoop Configuration)*

---

## Feature Engineering

The following business features were created:

- Shipping Days
- Order Year
- Order Month
- Order Quarter
- Profit Margin

---

## Spark SQL Analysis

Business analysis includes:

- Sales by Category
- Profit by Category
- Top Products
- Monthly Revenue
- Customer Segment Analysis
- Regional Performance
- State-wise Sales
- Shipping Performance
- Profit Margin Analysis
- Discount Analysis

---

## Project Structure
             Raw Retail CSV
                    │
                    ▼
           PySpark Data Ingestion
                    │
                    ▼
         Data Profiling & Validation
                    │
                    ▼
      Data Cleaning & Transformation
                    │
                    ▼
          Feature Engineering
                    │
                    ▼
            Spark SQL Analytics
                    │
        ┌───────────┴────────────┐
        ▼                        ▼
   Business Insights        Clean Dataset
