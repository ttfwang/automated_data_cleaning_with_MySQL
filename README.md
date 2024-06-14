# Automated Data Cleaning with MySQL

## Project Overview

This project focuses on developing an automated data cleaning process for US household income data using MySQL. The primary objective is to create a robust and efficient method to clean the dataset by removing duplicates, fixing data quality issues, and standardizing data entries. The project showcases the use of stored procedures, events, and triggers to automate the data cleaning process.

## Objectives

- **Automated Data Cleaning:** Implement an automated process to remove duplicates, correct errors, and standardize data for consistency.
- **Efficiency:** Ensure the data cleaning process is efficient and can handle new data additions without manual intervention.

## Data

The data used in this project is sourced from publicly available datasets containing household income information for various states and places in the US.

## Files in this Repository

- [README.md](https://github.com/ttfwang/automated_data_cleaning_with_MySQL): Documentation of the project.
- [Automated Data Cleaning_SQL script](https://github.com/ttfwang/automated_data_cleaning_with_MySQL/blob/main/Automated%20Data%20Cleaning_SQL%20script.sql): SQL script for automated data cleaning.
- [us_household_income.csv](https://github.com/ttfwang/automated_data_cleaning_with_MySQL/blob/main/raw_data-UeHOX.csv): Raw data file in CSV format.


## Automated Data Cleaning Process

The automated data cleaning process is implemented using stored procedures, events, and triggers:

1. **Stored Procedure:**
   - **Create Table:** Created a cleaned version of the table using `CREATE TABLE`.
   - **Copy Data:** Copied data from the original table to the cleaned table using `INSERT INTO`.
   - **Remove Duplicates:** Identified and removed duplicates using `ROW_NUMBER() OVER (PARTITION BY ...)`.
   - **Standardize Data:** Corrected typos and standardized entries using `UPDATE`.

2. **Event:**
   - Scheduled the stored procedure to run automatically every 30 days using `CREATE EVENT`.

3. **Trigger:**
   - Ensured the table is cleaned automatically when new data is added using `CREATE TRIGGER`.

## Conclusion

This project demonstrates the use of MySQL for automated data cleaning, showcasing skills in creating stored procedures, events, and triggers to ensure data consistency and efficiency.

## How to Use

1. Load the `us_household_income.csv` file into your MySQL database.
2. Run the `Automated Data Cleaning_SQL script` script to automate the data cleaning process.

## Acknowledgment

This project is a part of my self-learning journey to enhance my data analytic skills and transition to a data analyst role. This practice project is also a part of the data analytics lesson offered by [Analyst Builder](https://www.analystbuilder.com/courses/advanced-mysql-for-data-analysis/lesson/congratulations-VUQwO).

## Contact

Feel free to reach out via [LinkedIn](https://www.linkedin.com/in/tengfei-wang) or email me at tengfeiwang1989@gmail.com.
