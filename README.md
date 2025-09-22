# Sales Dataset Cleaning Process

This document outlines the steps followed to clean and prepare the sales dataset for analysis. The cleaning process ensures the dataset is reliable, consistent, and ready for downstream use such as analysis, visualization, or machine learning.

## 1. Handling Missing Values
- Inspected each column for missing or null values.
- Ensured no essential field contained unaddressed missing values.

## 2. Removing Duplicates
- Searched the dataset for duplicate rows based on all available columns.
- Removed all duplicate rows to guarantee each record is unique and no transaction is double-counted.

## 3. Correcting Data Types
- Verified all columns had the correct data types (numeric, categorical, string, etc.).
- Converted the **sales date** column to a `datetime` format to facilitate time-based operations.

## 4. Standardizing Categorical Values
- Standardized text data in key columns (e.g., `Payment_Method`, `Product_Category`):
  - Converted all text to consistent cases (lowercase or title case).
  - Trimmed extra spaces.
  - Corrected spelling, formatting, and capitalization inconsistencies.


## 5. Validating Value Ranges
- Ensured logical ranges for all columns:
  - Discounts limited between 0 and 1.
  - Quantities and sales amounts verified as non-negative.
- Corrected or flagged entries not conforming to logical business rules.

## 6. Review and Quality Checks
- Used `info()` and `describe()` methods to confirm remaining issues were addressed.
- Ensured the final dataset is **consistent, accurate, and ready for analysis or visualization** tasks.




