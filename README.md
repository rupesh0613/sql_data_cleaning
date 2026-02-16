# Global Tech Layoffs Data Cleaning Project (SQL)

## Project Overview

This project focuses on cleaning and preparing a real-world layoffs dataset using SQL.  
The dataset contains information about global tech layoffs during 2022.

The objective was to transform raw, inconsistent data into a structured and analysis-ready dataset by applying professional data cleaning techniques.

---

## Dataset Summary

- Source: Kaggle – Layoffs 2022 Dataset
- Records (Raw): 2361 rows
- Records (Cleaned): 1995 rows
- Features: 9 columns
- Time Period: 2022
- Domain: Global Tech Layoffs

---

## Data Cleaning Impact

- Initial Records: 2361
- Final Cleaned Records: 1995
- Total Rows Removed: 366
- Data Standardization Applied: Yes
- Duplicate Removal Method: ROW_NUMBER() Window Function
- Null Handling Strategy: Conditional Deletion & Data Imputation

This cleaning process improved dataset reliability and prepared it for accurate exploratory and time-series analysis.

---

## Cleaning Steps Performed

### 1. Removed Duplicates
Used `ROW_NUMBER()` window function inside a CTE to identify duplicate rows and removed them.

### 2. Standardized Text Data
- Trimmed whitespace
- Standardized country names
- Cleaned inconsistent industry values

### 3. Handled Missing Values
- Deleted rows where critical fields were NULL
- Used self-joins where applicable for filling missing values

### 4. Date Formatting
Converted date column into proper SQL DATE format for time-series analysis.

---


