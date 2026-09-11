# ASG Airlines – Flight Data Engineering & Analytics

## Project Overview

ASG Airlines Flight Data Engineering & Analytics is an end-to-end data engineering and business intelligence project designed to transform messy flight operational data into a reliable analytical dataset and an interactive Power BI dashboard.

The project addresses common real-world data challenges such as malformed flight IDs, inconsistent time formats, missing values, duplicate records, invalid durations, and overnight flights.

The solution uses Python and Pandas for data ingestion, validation, cleaning, transformation, and analytical preparation, followed by Power BI for interactive business intelligence and visualization.

---

## Business Problem

Airline operational data is often collected from multiple operational systems and may contain inconsistencies that affect reporting and decision-making.

The provided ASG Airlines dataset contained issues including:

- Malformed or invalid flight IDs
- Missing airline information
- Inconsistent date and time formats
- Duplicate or potentially duplicated records
- Invalid flight durations
- Overnight flights crossing calendar dates
- Data quality issues requiring validation before analysis

The objective of this project is to build a reliable data processing workflow that converts the raw operational data into a clean analytical dataset while preserving problematic records for auditability.

The final solution enables analysis of flight duration, airline distribution, route traffic, overnight operations, and data anomalies.

---

## Objectives

The major objectives of the project are to:

1. Ingest and inspect raw airline operational data.
2. Identify data quality problems during processing.
3. Validate and standardize flight IDs and time fields.
4. Handle missing and inconsistent values.
5. Correctly calculate flight duration, including overnight flights.
6. Detect abnormal or invalid flight records.
7. Prepare a structured analytical dataset.
8. Develop operational KPIs and analytical summaries.
9. Build an interactive Power BI dashboard.
10. Provide a scalable architecture for future cloud deployment.

---

## Technology Stack

| Technology | Purpose |
|------------|---------|
| Python | Data processing and transformation |
| Pandas | Data cleaning and analysis |
| NumPy | Numerical operations |
| Jupyter Notebook | Data engineering workflow |
| Microsoft Excel | Data storage and analytical output |
| Power BI | Interactive dashboard and visualization |
| DAX | KPI and analytical measures |
| GitHub | Version control and project documentation |

---

## Project Architecture

```text
Raw Flight Data
      │
      ▼
Excel / Raw Dataset
      │
      ▼
Python + Pandas
      │
      ├── Schema Validation
      ├── Flight ID Validation
      ├── Missing Value Handling
      ├── Duplicate Detection
      ├── Time Standardization
      ├── Overnight Flight Detection
      ├── Duration Calculation
      └── Anomaly Detection
      │
      ▼
Cleaned Analytical Dataset
      │
      ├───────────────┐
      ▼               ▼
Excel Analysis     Power BI
                      │
                      ▼
             Interactive Dashboard
                      │
                      ▼
             Business Insights
