# Zillow_Data_Analysis

**Objective:** The primary aim of this project is to build and automate a Python ETL process for extracting real estate property data from the Zillow Rapid API and loading it into AWS services for further transformation and visualization.

**Tools & Technologies:**

**Python:** Utilized for creating the ETL process

**Apache Airflow:** An open-source platform used for orchestrating and scheduling workflows. It will be installed from scratch during the project.

**AWS Services:** The project will extensively use various AWS services such as S3, Lambda, Redshift, and Quicksight.

**Zillow Rapid API:** The source of real estate property data.

Workflow:

**Data Extraction:** The data is extracted from the Zillow Rapid API

**Load to S3:** The extracted data is loaded into an Amazon S3 bucket

**Transformation with Lambda:** This action triggers a series of AWS Lambda functions to transform the data and convert it into CSV file format

**Load to Redshift:** Apache Airflow, utilizing an S3KeySensor operator, monitors and loads the transformed data into Amazon Redshift

**Visualization with Quicksight:** Amazon Quicksight is then connected to the Redshift cluster to visualize the data


The Architecture diagram:
![image](https://github.com/srijamannam/Data-Engineering-Project---Zillow-Data/assets/92010369/ee904bec-e7bf-4037-b9c6-69a839bd0ee6)

