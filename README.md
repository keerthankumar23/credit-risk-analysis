# credit-risk-analysis
# Credit Risk Analysis Pipeline

## Project Overview

This project implements an end-to-end Credit Risk Analysis data pipeline using Azure, Databricks, Delta Lake, dbt, Microsoft Fabric, and Power BI.

The pipeline follows the Medallion Architecture (Bronze → Silver → Gold) to ingest, transform, validate, and analyze credit risk data for business reporting and dashboard creation.

---

## Architecture

```
CSV Files
    │
    ▼
Azure Data Lake Storage (ADLS Gen2)
    │
    ▼
Azure Data Factory
    │
    ▼
Parquet Files
    │
    ▼
Databricks Bronze Layer
    │
    ▼
Databricks Silver Layer
    │
    ▼
dbt Gold Layer
    │
    ▼
Databricks SQL Warehouse
    │
    ▼
Microsoft Fabric / Power BI Dashboard
```

---

## Technologies Used

- Azure Data Lake Storage Gen2
- Azure Data Factory
- Azure Databricks
- PySpark
- Delta Lake
- Unity Catalog
- dbt Cloud
- Databricks SQL Warehouse
- Microsoft Fabric
- Power BI
- GitHub

---

## Project Workflow

### Bronze Layer
- Load raw parquet files
- Schema Evolution
- Watermarking
- Audit Logging
- Error Handling

### Silver Layer
- Data Cleaning
- Data Validation
- Remove Duplicates
- Handle Null Values
- Data Type Conversion
- Surrogate Key Generation
- SCD Type 2
- Delta Optimization
- Time Travel

### Gold Layer
- Star Schema
- Dimension Tables
- Fact Tables
- Business KPIs
- Aggregated Reports
- Dashboard Data Models

---

## Key Features

- End-to-End ETL Pipeline
- Medallion Architecture
- Incremental Processing
- Delta Lake
- SCD Type 2
- Time Travel
- Data Validation
- Business KPI Generation
- Power BI Dashboard

---

## Repository Structure

```
credit-risk-analysis/

├── ADF/
├── Bronze/
├── Silver/
├── Gold/
├── dbt/
├── PowerBI/
├── notebooks/
├── datasets/
└── README.md
```

---

## Future Enhancements

- Streaming Pipeline using Azure Event Hub
- Databricks Workflows
- Airflow Orchestration
- CI/CD using GitHub Actions
- Automated Data Quality Tests

---

## Author

**Keerthan Kumar**

Azure | Databricks | PySpark | dbt | Microsoft Fabric | Power BI
