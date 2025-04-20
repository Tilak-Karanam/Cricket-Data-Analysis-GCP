# 🏏 Cricket Batsmen Rankings Data Pipeline

This project automates the process of fetching, transforming, and loading cricket batsmen rankings data into Google BigQuery. The data is sourced from the CricBuzz API, processed, and uploaded to Google Cloud Storage (GCS) before being ingested into BigQuery for further analysis.

---

## 📌 Project Objectives

- Fetch batsmen rankings data from CricBuzz API
- Clean and transform the data into a structured format
- Upload the transformed data to Google Cloud Storage (GCS)
- Automate the data pipeline with Airflow
- Load the data into BigQuery for analytical purposes

---

## 🧠 Skills Demonstrated

- **API Integration**: Extracted batsmen rankings data using the CricBuzz API
- **Data Transformation**: Used JavaScript User-Defined Function (UDF) for transforming data before loading into BigQuery
- **Cloud Services**: Leveraged Google Cloud Storage, DataFlow, and BigQuery for storing, processing, and analyzing data
- **Data Pipeline Automation**: Implemented Airflow for scheduling and automating the ETL process
- **Data Loading**: Loaded data into BigQuery with defined schemas

---

## 🧰 Technologies Used

| Tool | Purpose |
|------|---------|
| Python | Core scripting language for fetching and processing data |
| Google Cloud Storage | Used to store the raw and processed data |
| Airflow | Orchestrates the data pipeline execution |
| DataFlow | Processes and loads data into BigQuery |
| BigQuery | Data warehouse for storing processed data |
| JavaScript (UDF) | Transforms CSV data to JSON before BigQuery loading |

---

## 🗂️ Project Files

- `dag.py`: Airflow DAG that automates the ETL pipeline
- `extract_and_push_gcs.py`: Fetches and processes data from CricBuzz API, uploads to GCS
- `extract_data.py`: Fetches and processes data from CricBuzz API without uploading to GCS
- `function.py`: Triggers Google DataFlow job to load data into BigQuery
- `trigger_df_job.py`: Python script that initiates the DataFlow job
- `udf.js`: JavaScript UDF for transforming data before loading into BigQuery
- `bq.json`: Defines the schema for the BigQuery table

---

## 🔍 Highlights

- Automated the daily fetch of cricket batsmen rankings using the CricBuzz API
- Uploaded processed data to Google Cloud Storage for later use in BigQuery
- Leveraged Airflow for scheduling and automating the ETL process
- Utilized Google DataFlow for processing and transforming the data into BigQuery-compatible format
- Built a fully automated, end-to-end data pipeline for BigQuery ingestion

---

## 🖼️ Data Model Overview

The data model for this project is based on a relational schema designed for the rankings data. The main tables include:
- **batsmen_rankings**: Stores the batsmen's rankings, names, and countries
- **BigQuery Schema**: Defines the table structure in BigQuery with fields such as `rank`, `name`, and `country`

The data is processed and loaded into BigQuery with this schema for further analysis and reporting.

---

## 🚀 Key Outcomes

- Successfully automated data extraction and loading into BigQuery
- Cleaned and transformed raw API data for storage in a relational model
- Developed a reliable, scalable data pipeline with minimal manual intervention
- Demonstrated strong end-to-end project management from data ingestion to reporting

---
