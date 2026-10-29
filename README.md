# AWS Cloud & Data Engineering Project

## Project Overview

This project demonstrates practical skills in **SQL, Linux commands, Amazon S3, AWS IAM, AWS Glue, and ETL data processing**. It covers database creation, SQL query execution, cloud storage, data cataloging, and data transformation using AWS services.

The project uses an electric vehicle (EV) charging database to practice SQL operations and demonstrates a cloud-based ETL workflow using Amazon S3 and AWS Glue.

## Objectives

- Create and query relational database tables using SQL.
- Perform data filtering, aggregation, sorting, and joins.
- Practice basic Linux commands for file and system management.
- Upload and store files in Amazon S3.
- Configure IAM roles and permissions for AWS services.
- Create an AWS Glue database and Data Catalog.
- Use Glue Crawlers to discover data schemas.
- Perform data transformation using AWS Glue Visual ETL.
- Understand the end-to-end cloud ETL pipeline.

## Technologies Used

| Technology | Purpose |
|---|---|
| SQL | Database creation, querying, and analysis |
| Linux | Basic file and system operations |
| Amazon S3 | Cloud storage for input and processed data |
| AWS IAM | Access control and service permissions |
| AWS Glue | Data cataloging and ETL processing |
| AWS Glue Crawler | Automatic schema discovery |
| AWS Glue Data Catalog | Metadata and table management |
| AWS Glue Visual ETL | Visual data transformation |

## Database Design

The project includes the following six tables for an electric vehicle charging system:

1. **customers** – Stores customer information.
2. **vehicles** – Stores vehicle details.
3. **charging_stations** – Stores charging station information.
4. **charging_points** – Stores charging point details and power capacity.
5. **charging_sessions** – Stores charging session and energy consumption information.
6. **payments** – Stores payment details and transaction information.

## SQL Queries Implemented

The project covers 15 SQL query tasks:

1. Find all vehicles manufactured by Tata.
2. Find charging stations located in Bengaluru.
3. Count the total number of customers.
4. Display successful payments from highest to lowest amount.
5. Count charging stations in each city.
6. Display vehicle registration numbers, brands, and owners' names.
7. Display station names and charger types.
8. Calculate successful payments for each payment method.
9. Find vehicles with battery capacity greater than 40 kWh.
10. Find customers who own more than one vehicle.
11. Calculate total energy consumed by each vehicle.
12. Find vehicles that consumed more than 30 kWh in total.
13. Find payment methods with more than three successful payments.
14. Identify vehicles with energy consumption greater than the average energy consumed per session.
15. Find charging points with power capacity greater than 50 kW.

These queries demonstrate filtering, sorting, aggregate functions, grouping, joins, subqueries, and conditional analysis.

## Linux Commands Practiced

The project includes basic Linux commands for navigating directories, managing files, and checking system information.

- `pwd` – Display the current working directory.
- `ls` – List files and directories.
- `ls -l` – Display detailed file information.
- `whoami` – Display the current username.
- `date` – Display the current date and time.
- `uname -a` – Display system information.
- `mkdir practice` – Create a directory.
- `cd practice` – Change the current directory.
- `touch notes.txt` – Create a file.
- `cat notes.txt` – Display file contents.
- `echo "Hello Linux" > notes.txt` – Write text to a file.
- `cp notes.txt backup.txt` – Copy a file.
- `mv backup.txt newfile.txt` – Rename or move a file.
- `df -h` – Display disk space usage.
- `vm_stat` – Display virtual memory statistics on macOS.

## AWS Implementation

### 1. Amazon S3

An S3 bucket is created to store the input files used in the data processing workflow. S3 acts as the cloud storage layer for the project.

### 2. AWS IAM

An IAM role is configured with the required permissions so AWS services can access the necessary resources.

### 3. AWS Glue Database

A database is created in AWS Glue to organize metadata about the datasets.

### 4. AWS Glue Crawler

A Glue Crawler is configured to inspect the data stored in S3, identify its structure, and create corresponding table metadata in the Glue Data Catalog.

### 5. AWS Glue Data Catalog

The Data Catalog maintains metadata such as table names, schemas, and data locations, making the datasets easier to discover and process.

### 6. AWS Glue Visual ETL

Glue Visual ETL is used to build a visual data processing workflow and configure data transformations.

### 7. Curated Data in S3

The intended output of the workflow is curated data stored in S3, ready for further analysis or downstream processing.

## ETL Workflow

The project's data processing workflow follows this sequence:

```text
Source Files
     |
     v
Amazon S3
     |
     v
AWS Glue Crawler
     |
     v
AWS Glue Data Catalog
     |
     v
AWS Glue Visual ETL
     |
     v
Data Transformation
     |
     v
S3 Curated Data
```

### Workflow Explanation

1. **Extract:** Upload source data files to an Amazon S3 bucket.
2. **Discover:** The AWS Glue Crawler scans the source data and identifies its schema.
3. **Catalog:** The Glue Data Catalog stores metadata about the discovered datasets.
4. **Transform:** AWS Glue Visual ETL is configured to process and transform the data.
5. **Load:** The transformed output is intended to be stored in an S3 curated-data location.

This workflow demonstrates how AWS services can be combined to build a cloud-based data processing pipeline.

## Learning Outcomes

Through this project, I gained practical exposure to:

- Writing SQL queries for data analysis.
- Understanding relationships between database tables.
- Using Linux commands for basic system operations.
- Working with Amazon S3 for cloud storage.
- Understanding IAM roles and permissions.
- Creating databases and tables in AWS Glue.
- Discovering schemas using Glue Crawlers.
- Understanding ETL concepts and data transformation workflows.
- Organizing source and curated data in a cloud environment.

## Conclusion

This project combines database management, Linux fundamentals, and AWS cloud services to demonstrate the basic concepts of cloud data engineering. It provides practical exposure to SQL-based data analysis and the design of an ETL workflow using Amazon S3 and AWS Glue.

## Author

 Kannaiahgari Tharun  

