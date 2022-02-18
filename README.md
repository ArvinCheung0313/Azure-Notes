# Azure-Notes
This is my notes of learning Azure.
Start Date: 2022-02-17

Learning is an active process. We learn by doing. Only knowledge that is used sticks in your mind.

:surfer:Currently updating...:surfing_man: 2020-02-17

# Contents
* [1 Overviews](#1-overviews)
  * [1.1 Azure Data Factory (ADF)](#11-azure-data-factory-adf)
  * [1.2 COVID-19 Prediction/Reporting](#12-covid-19-predictionreporting)
  * [1.3 Solution Architecture](#13-solution-architecture)
  * [1.4 Storage Solutions](#14-storage-solutions)

# 1 Overviews

## 1.1 Azure Data Factory (ADF)

### 1.1.1 ADF Is 
A fully managed, serverless data integration solution for ingesting, preparing and transforming all of your data at sacle. Basically, ADF provides an end to end solution for our data integration, transformation, and orchestration needs.
* **Ingestion**  
  Provides connectors to 90+ sources and it's increasing. For example, connectors for SAS applications are Salesforce, Office 365, also support for interesting data from other major cloud providers like Amazon S3 and Google Cloud Storage. It can also connect to SQL server.
* **Transformation/Analysis**  
  Still slightly limited functionality on ADF, thus we can create transformations in external solutions such as Spark.
* **Publish**  
  ADF also lets us orchestrate the publishing of dashboards created in tolls such as Power BI to Data Consumers.

### 1.1.2 ADF IS Not
* Data Migration Tool
* Data Streaming Service
* Suitable for Complex Data Transformations
* Data Storage Service

## 1.2 COVID-19 Prediction/Reporting

### 1.2.1 Objective
* **Prediction**
  Create a data platform from which our data science team can run machine learing models to predict the spread of the virus and find other insights from the data.
* **Reporting**  
  Create a data platform from which our data analysts can easily report on the COVID-19 trends using a reporting tool.
  
### 1.2.2 Data Lake
Data Lake to be built with the following data to aid Data Scientists to predict the spread of the virus/mortality
* Confirmed cases
* Mortality
* Hospitalization/ICU Cases
* Testing numbers
* COuntrys' population by age group

### 1.2.3 Data warehouse
Data warehouse to be built with the following data to aid Data Analysts to report on trends
* Confirmed cases
* Mortality
* Hospitalization/ICU Cases
* Testing numbers

### 1.2.4 Data Sources
* ECDC Website - [Link](https://www.ecdc.europa.eu/en/covid-19/data)
  * Confirmed cases
  * Mortality
  * Hospitalization/ICU Cases
  * Testing numbers
* Eurostat Website - [Link](https://github.com/ArvinCheung0313/Azure-Notes/blob/main/tps00010.tsv)
  * Population by age

## 1.3 Solution Architecture

<img width="981" alt="image" src="https://user-images.githubusercontent.com/91806768/154564103-c3a68287-2d24-483b-9b8b-ffddbd6a50db.png">

## 1.4 Storage Solutions

### 1.4.1 Key Factors to Consider
* Structure of the data
  * Structured
  * Semi-structured
  * Unstructured
* Operational needs
  * How often is the data accessed?
  * How quickly do we need to serve?
  * Need to run simple queries?
  * Need to run heavy analytical workload?
  * Accessed from multiple regions?
  * ...

### 1.4.2 Azure Databases
* Azure SQL Database
* Azure Databses for MySQL
* Azure Databse for PostgreSQL
* Azure Database for MariaDB
* VM Images with Oracle, SQL Server etc

### 1.4.3 Azure Storage Account
* Blob Storage: Can store unstructured data such as text files, media document, PDF etc.
* File Storage: Offers a fully managed cloud file store that can be accessed from anywhere via S&P protocal.
* Disk Storage
* Table Storage: Allows to store structured data in the form of key value pairs.
* Queue Storage: Can be used to store and retrieve messages from the queue.

### 1.4.4 Azure Data Lake Storage Gen 2
Designed to serve multiple petabytes of informaion while sustaining hundreds of gigabytes of input/output.
* Enhance Performance
* Enhance Management
* Better Security
* Inexpensive to Run









