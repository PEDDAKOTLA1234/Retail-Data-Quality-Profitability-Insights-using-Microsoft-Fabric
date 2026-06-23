# Retail Data Quality & Profitability Insights using Microsoft Fabric

## Project Overview

This project demonstrates an end-to-end analytics solution built on Microsoft Fabric using the Medallion Architecture pattern. The platform integrates Orders, Inventory, and Returns data from multiple operational systems into a centralized Lakehouse environment.

Using Microsoft Fabric Pipelines, Notebooks, OneLake, and Power BI, the solution performs data ingestion, cleansing, standardization, transformation, and business aggregations to generate trusted datasets for analytics and reporting.

The final Gold Layer provides business-ready data that enables stakeholders to analyze sales performance, inventory utilization, customer behavior, product returns, and profitability through interactive Power BI dashboards.

---

## Business Problem

Retail organizations often receive data from multiple systems with inconsistent formats, duplicate records, and missing values. These issues impact reporting accuracy and make it difficult to generate reliable business insights.

The objective of this project is to build a centralized analytics platform capable of:

* Integrating Orders, Inventory, and Returns datasets.
* Improving data quality through validation and cleansing.
* Monitoring inventory performance and stock movement.
* Tracking return behavior across products and categories.
* Measuring profitability and sales trends.
* Delivering executive-level dashboards through Power BI.

---

## Technology Stack

### Microsoft Fabric Components

* Fabric Lakehouse
* Fabric Data Factory
* Fabric Pipelines
* Fabric Notebooks
* OneLake
* Power BI

### Programming Languages

* PySpark
* SQL

### Data Engineering Concepts

* Medallion Architecture
* Incremental Processing
* Data Quality Framework
* Delta Tables
* Business Aggregations

---

## Solution Architecture

<img width="1693" height="929" alt="image" src="https://github.com/user-attachments/assets/18a3f96c-d275-4776-abef-86f44867b18b" />


---

# Part 1: Data Ingestion (Bronze Layer)

Data from Orders, Inventory, and Returns systems is ingested into Microsoft Fabric Lakehouse using Fabric Pipelines.

The Bronze Layer serves as the landing zone where source data is stored in its original format, ensuring historical preservation and auditability.

### Key Highlights

* Multi-source data ingestion.
* Incremental data processing.
* Automated pipeline execution.
* Raw data preservation.
* Delta table storage.
* Scalable ingestion framework.

### Business Value

Maintains a complete historical record of source data while providing traceability for auditing, troubleshooting, and reprocessing activities.



Fabric Pipeline
<img width="1908" height="890" alt="1000193957" src="https://github.com/user-attachments/assets/b946172c-19e0-4cbd-9279-86590922904b" />

 OneLake Storage
<img width="1901" height="906" alt="1000193982" src="https://github.com/user-attachments/assets/ea18f1b1-d7c9-4fd8-8392-2b408cc73334" />

Bronze Layer Tables
<img width="1915" height="853" alt="1000193961" src="https://github.com/user-attachments/assets/bb2f7fa3-7d81-4bb6-afb5-f9e2320911df" />
<img width="1246" height="356" alt="1000193964" src="https://github.com/user-attachments/assets/4fd99284-37ba-4025-ab2d-2fba3c936eaa" />



---

# Part 2: Data Transformation & Data Quality (Silver Layer)

The Silver Layer focuses on improving data quality and standardizing datasets using Fabric Notebooks and PySpark transformations.

Data quality checks and validation rules are applied before preparing data for downstream analytics.

### Transformations Performed

* Null value handling.
* Duplicate record removal.
* Schema validation.
* Data type standardization.
* Data cleansing and enrichment.
* Business rule implementation.

### Key Highlights

* Data quality framework implementation.
* Standardized and trusted datasets.
* PySpark-based transformations.
* Automated cleansing process.

### Business Value

Improves reporting accuracy and ensures business users work with reliable and consistent data.



Fabric Notebook
<img width="1919" height="891" alt="1000193958" src="https://github.com/user-attachments/assets/28316944-7e9d-455f-a8b5-f5d5c0409f51" />

Data Transformation Logic
<img width="1439" height="539" alt="1000193966" src="https://github.com/user-attachments/assets/094629ab-2885-42ba-b426-bcd9d226c896" />
<img width="1419" height="529" alt="1000193967" src="https://github.com/user-attachments/assets/100b9274-f9c1-4de4-bb7f-90b2ed2fb3dc" />
<img width="1429" height="330" alt="1000193968" src="https://github.com/user-attachments/assets/98fa8f2e-b0ee-4431-838a-aa7f0e079477" />



---

# Part 3: Business Aggregations (Gold Layer)

The Gold Layer contains curated and business-ready datasets optimized for analytics and reporting.

Business KPIs and aggregations are generated from cleansed data to support strategic decision-making.

### Metrics Generated

* Total Sales
* Net Profit
* Return Rate
* Inventory Turnover
* Average Order Value
* Product Profitability
* Customer Metrics

### Key Highlights

* Business aggregations.
* KPI generation.
* Delta table implementation.
* Analytics-ready datasets.

### Business Value

Provides a trusted source for executive reporting, operational monitoring, and profitability analysis.



Gold Layer Tables
<img width="1906" height="558" alt="1000193969" src="https://github.com/user-attachments/assets/a4680828-a463-44a6-bff8-d99370515895" />
<img width="1493" height="568" alt="1000193970 (1)" src="https://github.com/user-attachments/assets/c6552eee-b8d2-46a4-835c-a2a1a646cf0d" />
<img width="1498" height="686" alt="1000193971" src="https://github.com/user-attachments/assets/71b9defb-b170-4b76-a9af-3bf649459a88" />

KPI Calculation Outputs
<img width="1901" height="673" alt="1000193981" src="https://github.com/user-attachments/assets/92869546-3507-45d3-9e10-0cc8db9478e7" />



---


# Part 5: Power BI Reporting

Power BI dashboards were developed using Gold Layer datasets to provide business users with actionable insights.

### Dashboard Features

* Sales Performance Analysis
* Profitability Analysis
* Product Performance Tracking
* Inventory Monitoring
* Returns Analysis
* Executive KPI Dashboard

### Business Value

Enables data-driven decision-making through interactive visualizations and real-time business insights.


Monitoring Dashboard

<img width="1911" height="924" alt="1000193983" src="https://github.com/user-attachments/assets/1abad184-3be6-4e4d-9e14-0de35cafc700" />

<img width="1911" height="834" alt="1000193984" src="https://github.com/user-attachments/assets/0a1680e3-2bcc-414c-8be3-9aa6f27a68ea" />



---

# Conclusion

This project demonstrates the implementation of a modern retail analytics platform using Microsoft Fabric. By combining Medallion Architecture, Data Quality Frameworks, Incremental Processing, and Power BI reporting, the solution delivers reliable, scalable, and business-ready insights for operational and strategic decision-making.
