# Layoffs Analysis

### Project Overview

This data analysis project provides insights on the layoff of most companies from 2020 to 2023.

## Data Sources

Layoffs Data: The primary dataset used fro this analysis is the "layoffs_data.csv"file,containing detailed information about layoffs made by companies around the world.

### Tool

MYSQL

## Data Cleaning/Preparation

Data Loading

Data Cleaning :
Removing Duplicates
Standardizing Data
Removing null values or blank values
Remove Unwanted columns 

Exploratory Data Analysis

The exploratory data analysis involved exploring layoffs data to answer questions like;

- The max number laid.
- The year with the highest laid offs
- The Top 5 companies with the highest laid of from 2020 to 2023.
-Industries total laid off. 


Data Analysis

Some interesting Codes I worked with

``` sql

SELECT * 
ROW() OVER (PARTITION BY COMPANY,INDUSTRY,TOTAL_LAID_OFF,PERCENTAGE_LAID_OFF,COUNTRY,DATE) AS ROW_NUM
FROM LAYOFFS_STAGE3;
```

### References

Alexthe Analyst


### Result

1. The result of the data cleaning shoes that the maximum number of total laid of staff is 12000 and that was from  google.
2. The year with the highest sum of total laid of is 2023 with a total of 125677.
3. The industry with the highest laid of is consumer.
