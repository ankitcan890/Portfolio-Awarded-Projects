# Portfolio-Awarded-Projects

**Portfolio Project: AWS Data Analytics and Data Management for The City of Vancouver**
**Project Title: AWS Data Analytics Platform for Awarded Contracts in Vancouver** 
**Objective:**
The primary objective of this project is to design and implement a secure, efficient, and scalable data analytics platform using AWS services to analyze publicly awarded contracts in Vancouver. The goal includes data protection, governance, monitoring, and visualization to provide insights into the number and types of awarded contracts.

Dataset:
Contract data for the years 2022 and 2023, saved in Excel files named "awarddata2022" and "awarddata2023".
Additional data files extracted from the Vancouver website stored in AWS S3.
Methodology:
Data Storage Design:

Use AWS S3 to create three folders: curated, landing, and raw.
Store extracted contract data in the landing folder for analysis.
Data Preparation:

Use AWS Glue Data Brew to prepare the dataset.
Modify the schema for accurate data types and save processed data in a tabular format.
Create datasets: project1-contracts-dataset23-ankit and project1-contracts-dataset2022-ankit.
Data Ingestion:

Standardize data using AWS Glue Data Brew by addressing missing values and storing standardized data in the raw folder.
Data Pipeline Design:

Use AWS S3 for data storage.
Implement schema modifications to remove unnecessary columns.
Use union operations to combine data from different tables.
Perform aggregation to calculate values for the specified bid types.
Store the final results in the curated folder in S3.
Data Protection:

Use AWS Key Management Service (KMS) to create a symmetric key named "Project2-contracts-dataset2-ankit" for encryption and decryption.
Configure default encryption for the S3 bucket to ensure data protection.
Data Governance:

Establish data pipelines using AWS Glue.
Implement detection mechanisms to identify suspicious data using Canadian examples.
Filter data based on specific conditions and eliminate unnecessary columns for a clean dataset.
Data Monitoring:

Set up Amazon CloudWatch dashboards (e.g., "project2-contracts-dashboard-ankit") for monitoring costs and data usage.
Implement alarms using CloudWatch to notify when thresholds are exceeded.
Use CloudTrail to record user activities and modifications within the system.
Data Analysis:

Create databases and tables (e.g., "project2_awarded_table05_ankit") for storing and querying contract data.
Perform SQL queries to retrieve and analyze the data for insights.
Data Visualization:

Visualize bid types and counts using graphs.
Publish results on web servers for remote access and sharing.
Data Publishing:

Publish findings using a general server and a web server for accessibility.
Tools and Technologies:
Data Storage: AWS S3
Data Preparation: AWS Glue Data Brew
Data Protection: AWS KMS
Data Governance: AWS Glue, S3
Data Monitoring: Amazon CloudWatch, CloudTrail
Data Analysis: SQL (within AWS)
Visualization: Graphs generated from analyzed data
Deliverables:
A secure AWS S3 storage design with data encryption enabled.
Standardized datasets in the curated folder ready for analysis.
CloudWatch dashboard and alarms for monitoring.
Visual representations of the analysis results.
Published data accessible on web servers.
Timeline:
The expected completion time for this project is approximately 8-10 weeks, including phases for data storage setup, governance implementation, monitoring configuration, and final analysis.
