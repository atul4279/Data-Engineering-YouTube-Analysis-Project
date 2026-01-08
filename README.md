#YouTube Data Analysis – End-to-End Data Engineering Project
Project Overview

This project demonstrates an end-to-end data engineering pipeline built on AWS to analyze YouTube Trending Video data. The goal is to identify patterns and factors that influence video popularity—such as views, likes, comments, categories, and regions—to support data-driven advertising and content strategy decisions.

The project covers the complete lifecycle of data engineering: data ingestion, storage, cataloging, transformation, querying, and visualization.

#Business Objective

A company planning to invest in YouTube advertising wants to understand:

What type of videos trend on YouTube

Which categories perform best across regions

How user engagement metrics impact popularity

This project helps answer those questions by converting raw YouTube data into analytics-ready insights.

Dataset

Source: Kaggle – YouTube Trending Videos Dataset

Data Types:

CSV files: Video statistics (views, likes, comments, shares) by country

JSON files: Video category mappings

Data includes multiple regions such as US, Canada, Germany, France, India, etc.

Architecture

Cloud Platform: AWS

Services Used:

Amazon S3 – Data Lake (raw & processed data storage)

AWS IAM – Access control and security

AWS Glue

Crawlers for schema discovery

Glue Data Catalog for metadata management

Spark-based ETL jobs

Amazon Athena – SQL-based analytics on S3 data

AWS CLI – Programmatic interaction with AWS

Data Pipeline Flow

Ingest raw CSV and JSON files into Amazon S3

Organize data by region and data type

Use AWS Glue Crawlers to extract metadata and build tables

Perform ETL transformations using AWS Glue (Spark)

Query transformed data using Amazon Athena

Use query results to build analytical dashboards

Security Best Practices

IAM users created with least privilege principle

IAM roles used for service-to-service access

Root account protected with MFA

Data encrypted at rest in S3

Key Insights Enabled

Identification of top trending video categories

Regional comparison of video performance

Analysis of engagement metrics driving popularity

Actionable insights for YouTube ad campaign optimization

Key Concepts Learned

Big Data fundamentals

Data Lake vs Data Warehouse

Cloud vs On-Premise systems

Scalable ETL pipeline design

Metadata management and cataloging

Serverless analytics using Athena

How to Run the Project

Create an AWS account

Configure AWS CLI using IAM credentials

Create an S3 bucket for raw data

Upload Kaggle dataset to S3

Create AWS Glue Crawlers

Run ETL jobs using AWS Glue

Query data using Amazon Athena

Build dashboards using query results

Future Enhancements

Incremental data ingestion

Automation using AWS Step Functions

Integration with real-time streaming data

Advanced analytics and ML models
