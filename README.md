# Pharmaceutical Sales Performance Analysis

### Table of Contents
- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Tools](#tools)
- [Data Cleaning](#data-cleaning)
- [Exploratory Analysis](#exploratory-analysis)
- [Data Analysis](#data-analysis)
- [Reporting](#reporting)
- [Findings](#findings)
- [Recommendations](#recommendations)
  
##  Project Overview
This data analysis project aims to provide insights into the sales performance of a Germany-based pharmaceutical company over the 2022-2025 period. By analysing the various aspects of the sales, I seek to identify the revenues generated and trend (year-on-year) compared to the targets, distribution of the revenues by product-class, channels, and location, and the performance of the various sales teams. 

### Data Sources
The datasets used for this analysis consist of sales, target, employees, location, channels, and products data. Download links attached for your use.

### Tools
- Excel (dataset and data cleaning) [Download here] https:microsoft.com
- DAX functions
- PowerBI (dashboarding and modelling)

### Data Cleaning/Preparation
  In the initial data preparation stage, I carried out the following tasks
  1. Data loading and inspection
  2. Created 2 folders named "ETL" and "MODEL" to house the datasets for analysis after cleaning
  3. Appended the "Sales_2022" and "Sales_2023-2025" datasets and named the new table "Sales"
  4. Subsequently, the "Sales_2022" and "Sales_2023-2025" datasets were moved into the ETL folder, with Load-disabled.
  5. Merged "DimEmployees" and "Dim_Products" datasets with the new "Sales" table. This ensures that the product price and other necessary columns are brought into the Sales table.
  6. Merged the "Dim_Products" dataset with the "Target" table to incorporate the product prices.
  7. Data cleaning and formatting

### Exploratory Analysis
This involved exploring the data to answer questions pertinent to the sales performance of the company, such as:
 - What are the sales revenue and the quantity of products sold?
 - What is the year-to-date sales revenue?
 - What are the target revenue and the anticipated quantity of the products to sell?
 - How did the sales revenue change over the 2022-2025 period?
 - Which of the product classes generated the largest revenue?
 - Which sales channel and location accounted for the highest revenue?

### Data Analysis
DAX functions were used to determine the key performance indicators (measures), such as:
- SUM[Sales(Revenue)]
- SUM[Target(Revenue)]
- TOTALYTD([Sales Revenue],'Calendar'[Date])
- CALCULATE([Sales Revenue], SAMEPERIODLASTYEAR('Calendar'[Date]

### Reporting
A dashboard was built to visualize key performance indicators (KPIs) and answer other related questions. Similarly, a relationship model among the dataset variables was established. Meanwhile, the choice of colours for the dashboard and visuals was based on the colour elements of the company's logo.

### Findings
The findings of the analysis are summarised below:
  1. The company's sales revenue and volume exceeded the targets.
  2. The company experienced a year-on-year revenue growth, with 2024 being the best-performing year. 
  3.  Product classes such as analgesics, antiseptics, mood stabilizers, antipretics, and antibiotics accounted for the highest sales in volume and revenues.
  4. The largest quantities of the company's products were sold in Butzbach, Baeweller, Cuxhaven, Frieberg, and Neuss cities
  5.  Delta team, managed by Britanny Bold, was the best performing by sales revenue.
  6.  Volume of products sold has a direct relationship with revenues, provided the product prices remain the same or reviewed across the board.

### Recommendations
Based on the analysis, the following recommendations are necessary:
 1. The company should invest more in marketing and promotion during the low-peak sales months of January, April, and October.
 2. Focus on promoting the products in low-sales cities like Springe, Aurich, Schwelm, Oberrursel, and Weihl, without losing the grip on the high-sales cities.
 3. Incentivize the product distributors through commission.
㊗️🥇

