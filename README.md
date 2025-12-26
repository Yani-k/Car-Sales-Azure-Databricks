# Azure Data Engineering Project

## Overview

This project is an end-to-end Azure Data Engineering pipeline designed to implement real-world scenarios using the Medallion architecture. It covers key aspects such as incremental data loading, dimensional modeling (star schema), and handling slowly changing dimensions. The project ensures data governance, validation, audits, and logging, making it production-ready.


<img width="1413" height="623" alt="diagram-export-12-26-2025-12_29_10-AM" src="https://github.com/user-attachments/assets/30018988-a85a-4dd9-826b-34bb26bd5bdb" />


## Key Features

- **Azure Tech Stack**: Azure Data Lake, Azure SQL Database, Azure Data Factory, Azure Databricks, Unity Catalog, and Managed Identities.
- **Medallion Architecture**: Data is processed through Bronze (raw), Silver (transformed), and Gold (aggregated) layers.
- **Incremental Data Loading**: Uses Change Data Capture (CDC) to load only new data efficiently.
- **Dimensional Data Modeling**: Builds a star schema with fact and dimension tables.
- **Slowly Changing Dimensions (SCD)**: Implements SCD Type 1 (upsert) for managing historical data changes.
- **Production-Ready Pipelines**: Uses parameterized configurations for seamless deployment.

## Tools & Technologies

- **Storage & Processing**: Azure Data Lake, Azure Databricks
- **ETL & Data Orchestration**: Azure Data Factory
- **Data Management**: Azure SQL Database, Unity Catalog
- **Data Transformation**: PySpark, Delta Lake
- **Visualization**: Power BI&#x20;

## Project Workflow

1. **Data Ingestion**
   - Source data is stored in an Azure SQL Database (originally extracted from GitHub).
   - An initial pipeline loads historical data into the Bronze layer of Azure Data Lake.
   - Subsequent runs use an incremental data loading approach with stored procedures and CDC.
2. **Data Transformation**
   - Data moves from Bronze to Silver layer, undergoing cleansing and standardization.
   - The Silver layer data is processed into the Gold layer, structured into fact and dimension tables.
3. **Data Governance & Management**
   - Unity Catalog is used for data lineage and access control.
   - Data quality checks, audits, and logging are integrated.
4. **Data Consumption**
   - The transformed data in the Gold layer is ready for analytics and reporting.
   - Power BI can be connected for visualization.

## Deployment Steps

1. **Set up Azure Resources**
   - Create an Azure Data Lake storage account.
   - Set up an Azure SQL Database and load initial data.
   - Configure Azure Data Factory and Databricks.
2. **Develop ETL Pipelines**
   - Implement initial data load and incremental data pipeline.
   - Design and transform data using Medallion architecture.
3. **Run & Monitor Pipelines**
   - Deploy the pipeline and validate data flows.
   - Monitor job executions, logs, and error handling.

## Learning Outcomes

- Gain hands-on experience with an in-demand Azure data engineering stack.
- Understand real-world data pipeline design and implementation.
- Build scalable, production-ready ETL solutions with cloud services.
- Improve SQL and PySpark skills for data processing.

##
