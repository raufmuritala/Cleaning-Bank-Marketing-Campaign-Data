# Bank Marketing Campaign Data Cleaning & Database Preparation

## Project Overview
A comprehensive data cleaning and transformation project for a UK bank's personal loan marketing campaign data. Prepared raw customer data for PostgreSQL database integration by standardizing formats, converting data types, and structuring relational tables for future marketing campaigns.

## Project Description
Personal loans represent a significant revenue stream for UK banks, with typical interest rates around 10%. This project involved cleaning and structuring marketing campaign data from a major bank to enable efficient database storage and future campaign analysis. The cleaned data will support the bank's ongoing personal loan marketing initiatives and customer segmentation strategies.

## Technical Implementation

### Data Cleaning & Transformation
- **Data Standardization**: Converted job types and education levels by replacing periods with underscores
- **Boolean Conversion**: Transformed categorical responses ('yes'/'no', 'success') to boolean values for database efficiency
- **Missing Value Handling**: Replaced 'unknown' education values with proper NULL entries
- **Date Formatting**: Combined day and month columns into standardized datetime format with 2022 year reference

### Database Schema Preparation
Created three normalized tables for relational database storage:

#### client.csv
- Client demographic information (age, job, education, marital status)
- Financial indicators (credit default status, mortgage ownership)
- Unique client identifiers

#### campaign.csv
- Marketing engagement metrics (contact attempts, duration)
- Campaign performance data (current and previous outcomes)
- Temporal data with properly formatted contact dates

#### economics.csv
- Economic indicators (Consumer Price Index, EURIBOR rates)
- Macroeconomic context for campaign analysis

## Technologies Used
- **Python** (pandas, numpy)
- **Data Cleaning** & Transformation
- **Database Normalization**
- **CSV File Management**
- **PostgreSQL Preparation**

## Files
- `bank_marketing.csv` - Raw input data
- `client.csv` - Cleaned client demographic data
- `campaign.csv` - Cleaned marketing campaign data  
- `economics.csv` - Cleaned economic indicator data
- `bank_campaign_cleaning.ipynb` - Jupyter notebook with complete cleaning pipeline

## Usage
The cleaned datasets are ready for immediate import into PostgreSQL databases and will support:
- Customer segmentation analysis
- Marketing campaign performance tracking
- Economic impact assessment on loan uptake
- Future campaign data integration

