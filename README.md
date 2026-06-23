# Customer-Data-Cleaning-Project-Pandas (Python)

## Overview
This project focuses on cleaning and preparing a messy customer dataset using Python and Pandas.  
The dataset contains inconsistencies such as missing values, inconsistent formatting, duplicate entries, and mixed date formats.

The goal is to transform raw data into a clean, structured format suitable for analysis.


## Tools & Libraries
- Python 3
- Pandas

## Dataset Description
The dataset contains customer information with the following columns:

- CustomerID
- Name
- Age
- City
- Email
- Signup_Date

Issues in the raw dataset included:
- Inconsistent capitalization (e.g., "toronto" vs "Toronto")
- Missing values in Age, Email, and Signup_Date
- Mixed date formats (e.g., `2024-01-01`, `March 5 2024`, `01/02/2024`)
- Duplicate customer records
- Malformed CSV rows (extra commas in some fields)

```python
pd.read_csv("database_customers.txt", on_bad_lines="skip")
