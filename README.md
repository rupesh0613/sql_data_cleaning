# Global Tech Layoffs Data Cleaning Project (SQL)

## Project Overview

This project demonstrates advanced SQL-based data cleaning techniques applied to a real-world global layoffs dataset sourced from Kaggle.

The primary objective was to transform raw, inconsistent layoff records into a structured, analysis-ready dataset suitable for business intelligence, exploratory analysis, and time-series trend evaluation.

The project emphasizes practical data engineering skills using SQL, including duplicate removal, data standardization, null handling, and date transformation.

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

| Metric                | Value                                       |
| --------------------- | ------------------------------------------- |
| Initial Records       | 2,361                                       |
| Final Cleaned Records | 1,995                                       |
| Total Rows Removed    | 366                                         |
| Duplicate Handling    | ROW_NUMBER() Window Function                |
| Null Handling         | Conditional Deletion & Self-Join Imputation |
| Date Standardization  | Converted to SQL DATE format                |

---

## Impact Achieved

-Removed 366 inconsistent or duplicate records
-Improved dataset integrity and reliability
-Enabled accurate aggregation and time-series analysis
-Prepared clean data for analytical reporting

---

## Tech Stack

-SQL (MySQL)
-Window Functions (`ROW_NUMBER()`)
-Common Table Expressions (CTEs)
-Aggregate Functions
-Date Functions
-Data Standardization Techniques

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


