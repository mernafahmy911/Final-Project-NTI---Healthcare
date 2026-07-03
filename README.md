# 🏥 End-to-End Healthcare Fraud Detection Platform

## 📌 Overview

Healthcare fraud is a significant challenge that leads to financial losses, operational inefficiencies, and increased risks across healthcare systems. Detecting suspicious claims efficiently requires a combination of reliable data engineering, scalable analytics, and intelligent decision-making.

This project presents an end-to-end healthcare fraud detection platform designed to transform raw healthcare claims data into trusted analytical assets, actionable insights, and real-time fraud alerts. The solution combines traditional data warehousing, modern cloud architectures, streaming pipelines, machine learning, and business intelligence into a unified ecosystem.

---

## 🎯 Project Objectives

* Centralize healthcare claims data from multiple sources.
* Build scalable batch and streaming data pipelines.
* Enable reliable analytics and reporting.
* Detect potentially fraudulent claims using machine learning.
* Generate real-time fraud alerts.
* Support data-driven decision-making for healthcare stakeholders.

---

# 🏗 Solution Architecture

The platform was implemented through three complementary architectures to demonstrate different approaches to modern data engineering.

## 1️⃣ Data Warehouse Solution

A traditional data warehouse was designed using dimensional modeling principles to support analytical reporting and historical analysis.

### Key Components

* SSIS ETL Pipelines
* SQL Server Staging Layer
* Data Cleansing & Validation
* Dimensional Modeling
* Star Schema Design

📷 *Add Data Warehouse Architecture Image Here*

📷 *Add Star Schema Image Here*

---

## 2️⃣ Real-Time Streaming Solution

To support continuous data ingestion and near real-time processing, a streaming architecture was implemented.

### Key Components

* FastAPI Data Ingestion Service
* Apache Kafka Streaming Platform
* Snowflake Cloud Data Warehouse
* dbt Data Transformations
* Apache Airflow Orchestration

### Benefits

* Continuous data ingestion
* Automated transformations
* Scalable cloud architecture
* Reliable workflow orchestration

📷 *Add Kafka → Snowflake → dbt Architecture Image Here*

---

## 3️⃣ Lakehouse Architecture

A modern Medallion Architecture was implemented using Databricks and Delta Lake.

### Bronze Layer

* Raw healthcare claims data

### Silver Layer

* Cleansed and validated datasets
* Deduplication and quality checks

### Gold Layer

* Business-ready analytical datasets
* Optimized for reporting and advanced analytics

📷 *Add Databricks Medallion Architecture Image Here*

---

# 📊 Business Intelligence

Interactive dashboards were developed using Power BI to provide visibility into healthcare operations and fraud monitoring.

### Dashboard Capabilities

* Claims analysis
* Provider performance monitoring
* Fraud risk tracking
* Trend analysis
* Executive KPI reporting

📷 *Add Power BI Dashboard Screenshots Here*

---

# 🤖 Machine Learning Fraud Detection

A machine learning model was developed to identify potentially fraudulent healthcare claims and support proactive fraud investigation.

## Feature Engineering

Feature engineering techniques were applied to prepare and optimize the dataset for model training.

**Recursive Feature Elimination (RFE)** was used to evaluate feature importance and select the most relevant predictors, helping improve model performance while reducing unnecessary complexity.

## Model Development

The machine learning workflow included:

* Data preprocessing
* Feature engineering
* Feature selection using RFE
* Model training
* Model evaluation
* Fraud probability scoring

## Outcomes

The model generates fraud risk scores that help identify suspicious claims and prioritize investigations more effectively.

📷 *Add Model Performance / RFE Results Image Here*

---

# 🚨 Automated Fraud Alerting

To operationalize fraud detection, the machine learning model was integrated into an automated alerting workflow.

## Workflow

1. Claim data is submitted for evaluation.
2. The machine learning model predicts fraud probability.
3. n8n orchestrates the automation workflow.
4. Fraud alerts are generated automatically.
5. Results are delivered through a Telegram Bot.

## Benefits

* Near real-time fraud detection
* Automated alert generation
* Faster investigation workflows
* Improved operational response

📷 *Add n8n Workflow Screenshot Here*

📷 *Add Telegram Bot Screenshot Here*

---

# 🛠️ Technology Stack

| Category         | Technology     |
| ---------------- | -------------- |
| ETL              | SSIS           |
| Database         | SQL Server     |
| Streaming        | Apache Kafka   |
| API              | FastAPI        |
| Data Warehouse   | Snowflake      |
| Transformation   | dbt            |
| Orchestration    | Apache Airflow |
| Lakehouse        | Databricks     |
| Storage          | Delta Lake     |
| Machine Learning | Python         |
| Model Serving    | Flask          |
| Automation       | n8n            |
| Notifications    | Telegram Bot   |
| Visualization    | Power BI       |

---

## 🎓 About This Project

This project was completed as the **Final Project of the Data Engineering Track at the National Telecommunication Institute (NTI)**.

It demonstrates the integration of Data Engineering, Data Warehousing, Cloud Analytics, Business Intelligence, and Machine Learning concepts within a production-style healthcare fraud detection platform.
