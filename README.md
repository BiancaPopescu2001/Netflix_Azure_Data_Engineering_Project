<h1 align="center">Netflix Azure Data Engineering Project</h1>

![Text](https://github.com/BiancaPopescu2001/Netflix_Azure_Data_Engineering_Project/blob/main/cover_pic.jpg)

## 📘 Table of Contents
- [Introduction](#introduction)
- [Architecture](#architecture)
- [Data Dictionary](#data-dictionary)
- [Skills Demonstrated](#skills-demonstrated)

---

## Introduction
This project focuses on building a data engineering pipeline for Netflix data using the Azure ecosystem.

## Architecture

The project follows a modern medallion data architecture (**Bronze–Silver–Gold**) built entirely on Microsoft Azure.

Azure Data Factory (ADF) orchestrates the data ingestion process:

  - Connects to GitHub through a web activity to fetch raw Netflix datasets.

  - Copies data files (netflix_cast, netflix_countries, netflix_directors, netflix_category, netflix_titles) into the Bronze container of Azure Data Lake Storage Gen2.

Azure Databricks handles the data transformation and enrichment stages:

  - The Bronze layer stores raw ingested data using Databricks Auto Loader for incremental updates.

  - The Silver layer refines and cleans data (handling nulls, adding flag columns, splitting fields) and saves it in Delta format for optimized access.

  - The Gold layer, implemented with Delta Live Tables (DLT), organizes the final transformed data into curated tables ready for analytics and reporting.

The entire pipeline is modular, scalable, and automated, enabling reliable data movement and transformation within the Azure ecosystem.

## Data Dictionary
Data dictionary details here...

## Skills Demonstrated
- Azure Cloud Architecture
- Data Ingestion
- ETL Orchestration
- Delta Lake Architecture
- Delta Live Tables (DLT)



  





