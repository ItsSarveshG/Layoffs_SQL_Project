**SQL Project 1: World Layoffs Data Cleaning**

*Project Overview*

This project focuses on cleaning and preparing real-world layoff data using SQL.
The dataset contains company layoff information across countries, industries, and time periods.
The goal was to transform raw, inconsistent data into a clean, analysis-ready dataset.


**SQL Project 2: Exploratory Data Analysis (EDA) – World Layoffs**

*Project Overview*

This project performs Exploratory Data Analysis (EDA) on the cleaned layoffs dataset to uncover
trends, patterns, and insights related to global layoffs.

**Dataset**
Source: Kaggle – World Layoffs Dataset (2020–2023)
Data Type: Company, industry, country, total laid off, percentage laid off, date
Database Used: MySQL

**Project 1 Objectives**

Create a safe staging environment for data cleaning
Identify and remove duplicate records
Handle null and inconsistent values
Standardize text fields (company, industry, country)
Convert and validate date formats
Prepare a clean table for EDA and reporting

**Project 2 Objectives**

Identify companies, industries, and countries most affected by layoffs
Analyze layoffs by year and time trends
Detect outliers and extreme layoff events
Understand how layoffs evolved during different periods

**** PROJECT 1 ****

*Key SQL Techniques Used*

CREATE TABLE & staging tables
ROW_NUMBER() with PARTITION BY for duplicate detection
CTE (Common Table Expressions)
TRIM(), UPPER(), string standardization
NULL handling & conditional updates
Date formatting & validation
Data integrity checks

*Data Cleaning Steps*

Created staging tables to preserve raw data
Removed exact and logical duplicates
Standardized:
1. Company names
2. Industry labels
3. Country names
Converted date columns into proper SQL date format
Removed rows with no meaningful layoff information

*Outcome*

Cleaned and structured dataset ready for analysis
Improved data accuracy and consistency
Enabled meaningful exploratory and trend analysis


**** PROJECT 2 ****

*Key SQL Techniques Used*

GROUP BY & aggregate functions (SUM, MAX)
Date functions (YEAR)
Sorting & ranking
Filtering for high-impact events
Trend-based analysis

*Key Analysis Performed*

Total layoffs by:
1.  Company
2.  Industry
3.  Country
4.  Location
Year-wise layoffs trend
Largest single layoff events
Identification of sectors most impacted

*Insights Generated*

Certain industries and countries were disproportionately impacted
Layoffs peaked during specific years
A small number of companies contributed to a large share of total layoffs
