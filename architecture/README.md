# Project Architecture

## Overview
The Rapido Ride Analysis project uses Microsoft Azure services to build a data analytics pipeline and generate meaningful insights from ride-booking data.

## Architecture Components

1. **Azure Data Lake Storage Gen2 (ADLS):** Stores raw and transformed datasets.
2. **Azure Data Factory (ADF):** Orchestrates the data processing workflow.
3. **Azure Databricks:** Performs data cleaning, transformation, and analysis using PySpark.
4. **Azure SQL Database:** Provides a database integration component for analytical data.
5. **Power BI:** Creates interactive dashboards to visualize ride-booking insights.

## Medallion Architecture

- **Bronze Layer:** Stores raw ride-booking data.
- **Silver Layer:** Cleans and transforms the data and derives useful columns such as Month and Is_Weekend.
- **Gold Layer:** Prepares curated analytical outputs for reporting.

## Data Pipeline Workflow

1. Raw data is stored in ADLS Gen2.
2. Azure Data Factory triggers the Databricks notebook activities.
3. Databricks processes the data through Bronze, Silver, and Gold layers.
4. Curated outputs are prepared for analytical reporting.
5. Power BI presents the results through an interactive dashboard.

## Dashboard Insights

The dashboard focuses on:
- Total revenue and total rides
- Completed bookings
- Average surge
- Revenue by city
- Booking status distribution
- Vehicle type analysis
- Ride demand by hour

## Conclusion

This architecture combines cloud data storage, data engineering, and business intelligence to analyze ride-booking patterns and present useful insights.
