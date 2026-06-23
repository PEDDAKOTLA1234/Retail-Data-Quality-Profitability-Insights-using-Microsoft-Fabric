# Retail-Data-Quality-Profitability-Insights-using-Microsoft-Fabric

Project Overview

A retail organization receives Orders, Inventory, and Returns data from multiple operational systems. Due to inconsistent formats, duplicate records, and missing values, business users struggle to generate reliable insights.

This project leverages Microsoft Fabric and the Medallion Architecture pattern to build a scalable analytics platform that cleanses, standardizes, enriches, and aggregates retail data into business-ready datasets.

The final Gold Layer serves as a trusted source for Power BI dashboards that provide insights into sales performance, inventory health, customer behavior, return patterns, and profitability.

Business Problem

The organization requires a centralized analytics platform capable of:

Integrating Orders, Returns, and Inventory datasets.
Improving data quality through cleansing and validation.
Tracking profitability across products and categories.
Monitoring return behavior.
Measuring inventory efficiency.
Delivering executive dashboards through Power BI.
Technology Stack
Microsoft Fabric Components
Fabric Lakehouse
Fabric Data Factory
Fabric Pipelines
Fabric Notebook
OneLake
Power BI
Languages
PySpark
SQL
Architecture
Medallion Architecture
Incremental Processing
Delta Tables
Solution Architecture

📷 Attach Architecture Diagram Here

Part 1: Data Ingestion (Bronze Layer)

Data from Orders, Inventory, and Returns systems is ingested into the Bronze Layer using Microsoft Fabric Pipelines.

The Bronze Layer acts as the landing zone and stores source data in its original form.

Key Highlights
Multi-source ingestion.
Raw data preservation.
Delta table storage.
Incremental data ingestion.
Automated pipeline execution.
Business Value

Maintains a complete historical copy of source data and provides traceability for auditing and debugging purposes.

📷 Screenshots

Fabric Pipeline
OneLake Storage
Bronze Tables
Part 2: Data Transformation (Silver Layer)

The Silver Layer focuses on improving data quality and creating standardized datasets.

Activities Performed
Null value handling.
Duplicate removal.
Schema validation.
Data standardization.
Data enrichment.
Business rule implementation.
Business Value

Provides clean and reliable datasets for analytical workloads.

📷 Screenshots

Fabric Notebook
Silver Layer Tables
Transformation Logic
Part 3: Business Aggregations (Gold Layer)

The Gold Layer contains curated business datasets optimized for reporting and analytics.

Metrics Generated
Total Sales
Return Rate
Average Order Value
Inventory Turnover
Net Profit
Product Profitability
Unique Customers
Business Value

Provides a trusted and analytics-ready data model for business stakeholders.

📷 Screenshots

Gold Layer Tables
KPI Calculations
Part 4: Data Modeling & Optimization

Business-ready tables were modeled to support high-performance analytical queries.

Key Features
Delta Tables
Optimized Storage
Partitioning
Query Performance Optimization

📷 Screenshots

Data Model
Relationships
Part 5: Power BI Reporting

Power BI dashboards were created directly from Gold Layer tables.

Dashboard Features
Sales Analysis
Profitability Analysis
Product Performance
Inventory Monitoring
Return Analysis
Executive KPI Dashboard

📷 Screenshots

Dashboard Overview
KPI Dashboard
Profitability Dashboard
Part 6: Pipeline Orchestration & Incremental Processing

Fabric Pipelines were used to orchestrate the complete workflow.

Features
Automated execution.
Dependency management.
Incremental processing.
Monitoring and logging.

📷 Screenshots

Pipeline Flow
Pipeline Execution Results
Key Business Insights
Identified high-return product categories.
Measured profitability by product and category.
Tracked inventory performance.
Analyzed customer purchasing behavior.
Monitored revenue and profit trends.
Improved data quality across operational systems.
