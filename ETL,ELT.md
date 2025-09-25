# ETL (Extract, Transform, Load)

* Definition: Traditional data integration process where data is extracted from multiple sources, transformed into a proper format/structure, and then loaded into a target system (like a data warehouse).

## Steps:

* Extract
Pull data from heterogeneous sources (databases, APIs, files, sensors, etc.). Ensures raw data collection.
* Transform
Clean, standardize, filter, aggregate, and apply business rules. Data is transformed before loading.
* Load
Store the transformed data into the target system (usually a data warehouse).

## Characteristics:

* Data is cleaned & standardized before loading.
* Transformation happens in a staging area.
* Used when data quality and business rules are critical.
* More resource-heavy on the ETL tool or middleware.

## Example Tools:
* Informatica, Talend, Pentaho, IBM DataStage, SSIS.

# ELT (Extract, Load, Transform)

* Definition: Modern approach where data is extracted from sources, directly loaded into the target system (often a cloud-based data lake/warehouse), and then transformations are applied within the warehouse.

## Steps:

* Extract
Data pulled from sources.
* Load
Load raw data directly into the target system.
* Transform
Transformations are executed inside the data warehouse using its processing power (e.g., SQL, cloud services).

## Characteristics:

* Data is loaded in raw form first, transformations later.
* Efficient when using cloud warehouses (Snowflake, BigQuery, Redshift).
* Better scalability for big data.
* Shifts workload to the target system (which is usually highly optimized).

## Example Tools:
* Fivetran, Stitch, Airbyte, dbt (for transformations).

## Key Differences Between ETL and ELT
![Capture 14](https://github.com/user-attachments/assets/cfec88e2-13f2-4039-93c7-47fb7089b8cd)

## When to Use

## ETL
* On-premises warehouses.
* Data requires strict cleaning before storage.
* Legacy systems.

## ELT

* Cloud-native architectures.
* Huge datasets (IoT, clickstream, logs).
* When storage is cheap, and compute is scalable.

# DATA WAREHOUSING OLAP VS OLTP DIMENSIONAL MODELING

## Data Warehousing
## "A data warehouse is subject-oriented, integrated, time-variant, and non-volatile collection of data in support of management's decision-making process."

* A central repository of integrated data from disparate sources.
* Designed for analysis and reporting, not daily operations.
* Provides a historical, consistent, and subject-oriented view of data.
* The backbone for business intelligence and decision-making.


## Need for Data Warehousing

* Handles large data volumes (MBs/GBs → TBs).
* Supports complex analytics beyond transactions.
* Provides centralized storage (single source of truth).
* Enables trend analysis us
* Powers Business Intellige driven decisions.


## Characteristics of Data Warehousing

* Subject-Oriented focussed on buisiness subjects (sales, customers)
* Integrated → Data comes from multiple sources, standardized.
* Time-Variant→ Stores historical data for trend analysis.
* Non-Volatile → Once entered, data is stable and rarely changes.

## Components od Data Warehousing

* Data Sources: Operational systems, databases, external feeds.
* ETL (Extract, Transform, Load): Cleans & loads data. Data Warehouse Database: Central, structured repository.
* Metadata: Describes data’s structure, source, usage.
* Data Marts:Department-specific subsets.
* OLAP Tools: Multi-dimensional analysis.
* End-User Tools: Dashboards, BI & reporting tools.

  ![Capture16](https://github.com/user-attachments/assets/a1981be7-64e3-438d-9dbe-1520ca53da40)


## EXAMPLE OF DATA WAREHOUSIING
1. E-commerce: Flipkart
* Data Gathering: Orders, returns, payments, user clicks, delivery updates.
* Schema: Combines source data into a structured star schema for analysis.
* Cleansing: Standardizes customer names, locations, and product categories.
* Updates: Near real-time or scheduled loads for fresh insights.
* Summarization: Bestsellers by category, regional demand trends, logistics performance.

2. Banking: HDFC Bank
* Data Gathering: ATM transactions, online banking, credit card usage, loan records.
* Schema: Integrates data from core banking, CRM, and fraud detection systems.
* Cleansing: Fixes inconsistencies in account info, transaction logs, and addresses.
* Updates: Transaction data is batched and uploaded nightly.

 ## Database vs. Data Warehouse vs. Data Lakes 
![Capture15](https://github.com/user-attachments/assets/9d8b22a1-7015-4d2a-9389-3e1000b66763)


# OLTP 
## Characteristics:
* Focus: Fast, frequent INSERT, UPDATE, DELETE operations.
* Data Model: Highly normalized (to reduce redundancy and ensure data integrity).
* Users: Thousands of concurrent users (e.g., cashiers, online shoppers).
* Data: Current, detailed operational data.

  
## Example:
* ATM withdrawals, online order
* placement, airline ticket booking.

## Purpose:
* Designed for day-to-day operations (e.g., banking transactions, retail sales, reservations).













