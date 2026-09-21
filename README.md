# Sales Data Cleaning — SQL Server

## Overview

This project focuses on cleaning and validating a raw sales dataset using **SQL Server**.

The goal was to identify data-quality issues and prepare the dataset for further analysis and dashboarding.

## Data Quality Issues

The raw data contained issues such as:

* Missing values
* Duplicate transactions
* Invalid dates
* Negative quantities
* Incorrect or inconsistent values
* Inconsistent payment methods
* Mismatched `price × quantity` and `total_amount`

## What I Did

* Loaded the raw CSV data into SQL Server.
* Checked NULL values across all columns using dynamic SQL.
* Identified duplicate transaction IDs.
* Validated and cleaned invalid dates using `TRY_CONVERT()`.
* Handled negative quantities using business rules.
* Checked revenue calculation consistency.
* Standardized inconsistent categorical values.
* Kept the raw data unchanged and performed cleaning separately.

## Tools Used

* **SQL Server / SSMS**
* **SQL**
* CSV dataset

## Outcome

The cleaned dataset is now ready for **SQL analysis and Tableau dashboarding**, with the major data-quality issues identified and addressed.

## Project Structure

```text
Sales-Data-Cleaning/
│
├── data/
│   └── sales.csv
│
├── sql/
│   ├── 01_Data_Quality.sql
│   └── 02_Data_Cleaning.sql
│
└── README.md
```
