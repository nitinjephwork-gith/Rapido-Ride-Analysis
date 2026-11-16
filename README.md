
# Rapido Ride Analysis

## Project Overview

Rapido Ride Analysis is a data engineering and business intelligence project designed to organise, process and analyse ride-related operational data using Microsoft Azure services and Power BI.

The project follows a cloud-based data workflow in which source records are ingested, stored in structured layers, transformed using Azure Databricks and PySpark, and presented through an interactive Power BI dashboard.

The dashboard provides insights into ride volume, revenue, booking status, pickup locations, vehicle categories and surge indicators.

## 🎥 Project Demo

Watch the project demonstration on YouTube:

[**Rapido Ride Analysis – YouTube Demo**](https://youtu.be/SXeYLKYgYWo)

## Project Objectives

- Organise ride-related source data for analysis.
- Implement a Bronze, Silver and Gold data storage architecture.
- Use Azure Databricks and PySpark for data transformation.
- Orchestrate notebook execution through Azure Data Factory.
- Prepare analytical outputs for business intelligence.
- Develop an interactive Power BI dashboard.
- Analyse ride activity across cities, booking statuses and vehicle types.

## Technology Stack

| Technology | Purpose |
|---|---|
| Microsoft Azure | Cloud platform |
| Azure Data Factory | Data pipeline orchestration |
| Azure Data Lake Storage Gen2 | Layered data storage |
| Azure Databricks | Data processing environment |
| Python / PySpark | Data transformation |
| Azure SQL Database | Relational database component |
| Microsoft Power BI | Data visualisation and reporting |

## System Architecture

The project follows a Medallion Architecture consisting of three data layers:

### 1. Bronze Layer
Stores the ingested source data in its raw form.

### 2. Silver Layer
Contains refined and transformed records. The demonstrated transformations include deriving calendar attributes such as Month and Is_Weekend.

### 3. Gold Layer
Contains curated analytical outputs prepared for reporting and dashboard consumption.

### Overall Workflow

1. Identify the source data.
2. Ingest and organise records using Azure services.
3. Store data in the Bronze layer.
4. Transform records using Azure Databricks and PySpark.
5. Prepare curated outputs in the Gold layer.
6. Orchestrate processing activities using Azure Data Factory.
7. Present analytical results through Power BI.

## Azure Data Factory Pipeline

The project includes an Azure Data Factory pipeline named `RapidoRidePipeline`.

The visible pipeline contains Bronze, Silver and Gold notebook activities, followed by downstream copy activities for analytical outputs such as:

- Revenue
- Surge
- Peak Hour
- Vehicle
- Booking Status

The report documents successful execution indicators for the visible pipeline activities.

## Power BI Dashboard

The Power BI dashboard provides an interactive overview of ride operations.

### Key Dashboard Features

- **Total Revenue:** Displays the revenue represented in the dataset.
- **Total Rides:** Shows the overall number of rides.
- **Completed Bookings:** Displays completed ride bookings.
- **Average Surge:** Shows the average surge indicator.
- **Revenue by City:** Compares revenue across Delhi, Hyderabad, Bengaluru, Chennai and Pune.
- **Booking Status Distribution:** Compares completed, cancelled and incomplete bookings.
- **Vehicle Type Distribution:** Shows the distribution of Auto and Bike categories.
- **Ride Demand by Hour:** Provides a time-based ride analysis visual.
- **Interactive Filters:** Allows filtering by pickup location, vehicle type and booking status.

## Project Structure

```text
rapido-ride-analysis/
│
├── README.md
│
├── architecture/
│   └── README.md
│
├── notebooks/
│   └── README.md
│
├── sql/
│   └── README.md
│
└── screenshots/
    └── README.md
```


## Key Outcomes

- Demonstrated a cloud-based data engineering workflow.
- Organised ride data using the Medallion Architecture.
- Used Azure Databricks and PySpark for data preparation.
- Coordinated notebook execution through Azure Data Factory.
- Developed a Power BI dashboard for descriptive ride analytics.
- Presented operational indicators through interactive visualisations.

## Future Enhancements

- Verify and complete the Azure SQL data-loading integration.
- Improve data quality checks and pipeline monitoring.
- Validate the ride-demand chart's field assignments.
- Add automated pipeline scheduling.
- Explore advanced demand analysis and forecasting.

## Conclusion

Rapido Ride Analysis demonstrates the application of cloud data engineering and business intelligence tools to ride-related operational data. By combining Azure services, PySpark and Power BI, the project provides a structured workflow for data preparation and interactive reporting.

---

Project Domain: Data Engineering & Analytics
Project Type: Academic / Industrial Training Project
Technologies: Microsoft Azure, Databricks, Python, PySpark, SQL and Power BI
Developed by: Nitin kumar jeph
