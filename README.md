# Scalable Sports Data Pipeline & Analytics Platform on Azure ⚡

This project demonstrates a production-grade, cloud-native data pipeline on Microsoft Azure, built to ingest, process, and analyze over 100 GB of structured sports performance data. The solution is highly scalable, cost-optimized, and leverages modern data tools for continuous data updates and advanced analytics.

## 🏗️ Architecture Overview

- **Data Source:** Public sports telemetry and performance APIs (JSON/CSV)
- **Ingestion & Orchestration:** Azure Data Factory
- **Processing:** Azure Databricks (PySpark)
- **Data Warehouse:** Azure Synapse Analytics
- **Scheduling:** Weekly ETL refresh via ADF triggers
- **Monitoring:** ADF Pipeline monitoring + logging

<p align="center">
  <img src="https://github.com/user-attachments/assets/2cb0a34d-1845-47fd-9c06-911384c5ba3b" alt="Architecture Diagram" width="600"/>
</p>

## 🔄 ETL Flow

1. **Extract:** Pull raw data from public API endpoints using ADF
2. **Transform:** Handle schema normalization, cleansing, and feature engineering in Databricks
3. **Load:** Load curated datasets into Synapse for downstream analytics
4. **Automate:** Trigger workflows on a weekly cadence for fresh insights

## 📊 Highlights

- Ingested and processed over **100 GB** of multi-source data
- Reduced data storage footprint by **40%** through Delta optimization
- Achieved **20% cost savings** through efficient Spark job configuration
- Enabled near real-time analytics through Azure Synapse
- Implemented robust scheduling for **weekly pipeline refresh**
