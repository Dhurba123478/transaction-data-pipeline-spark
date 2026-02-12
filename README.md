# Transaction Medallion Architecture (Databricks + Spark)

## Overview
This project implements a simplified Medallion Architecture (Bronze, Silver, Gold) using PySpark and Delta Lake in Databricks.

## Architecture
Bronze → Raw transactions
Silver → Cleaned and deduplicated transactions
Gold → Aggregated daily customer metrics

## Technologies Used
- Apache Spark (PySpark)
- Delta Lake
- Databricks

## Key Features
- Data quality checks (null and negative amount removal)
- Deduplication using window functions
- Incremental-friendly architecture
- Business-level daily aggregations

## Layers
### Bronze
Raw transaction storage

### Silver
Cleaned, validated, deduplicated records

### Gold
Daily customer spend metrics
