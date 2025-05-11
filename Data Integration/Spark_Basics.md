# Getting Started with Apache Spark and Spark SQL

## Environment Setup

- Set up a Spark development environment using one of the following:
  - Databricks Community Edition (recommended for beginners)
  OR
  - Local installation via PySpark in Jupyter Notebook or IntelliJ

## Task 1: Load Data into RDD

- Use a small CSV or TXT file (e.g., sample log or text file)
- Read the file using SparkContext and create an RDD
- Perform basic operations:
  - Count number of lines
  - Filter lines containing a specific word
  - Display the first 5 lines

## Task 2: Work with DataFrames

- Read a structured CSV file as a Spark DataFrame
- Display schema and first few rows
- Use `.select()`, `.filter()`, and `.groupBy()` to perform simple queries
- Register the DataFrame as a temporary view and run a few SQL queries using `spark.sql()`
