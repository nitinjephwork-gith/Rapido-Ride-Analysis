# Databricks Notebooks

This folder is intended to contain the Azure Databricks notebooks used in the Rapido Ride Analysis project.

## Notebook Workflow

The project follows three main stages of data processing:

### 1. Bronze Layer – Data Ingestion
- Loads the raw ride-booking dataset.
- Stores the original data in the Bronze layer.

### 2. Silver Layer – Data Transformation
- Cleans and transforms the raw dataset.
- Derives additional columns such as Month and Is_Weekend.
- Prepares the data for further analysis.

### 3. Gold Layer – Data Analysis
- Creates curated analytical outputs.
- Prepares data for reporting and dashboard development.

## Tools Used
- Azure Databricks
- Python
- PySpark
- Azure Data Lake Storage Gen2

## Note
The original Databricks notebook source files will be added to this folder when available. This README currently documents the notebook workflow followed in the project.
