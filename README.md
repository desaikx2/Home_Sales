# Home_Sales

# Home Sales Analysis with Spark SQL

This notebook demonstrates how to use Spark SQL to analyze a dataset of home sales.

## Overview

The notebook performs the following steps:

1. Reads a CSV file of home sales data from an AWS S3 bucket into a Spark DataFrame.
2. Creates a temporary view of the DataFrame to enable SQL queries.
3. Calculates the average price of homes based on various criteria, such as number of bedrooms, bathrooms, and square footage.
4. Caches the temporary table to improve query performance.
5. Compares the runtime of queries using cached and uncached data.
6. Partitions the data by the "date_built" field and saves it in Parquet format.
7. Reads the Parquet data and creates a temporary table.
8. Compares the runtime of queries using Parquet data to cached and uncached data.
9. Uncaches the temporary table.

## Requirements

- Google Colab environment
- Spark 3.5.3
- Java 11
- Python 3.x
- `findspark`
- `pyspark`
- `time`
- `os`

## Usage

1. Open the notebook in Google Colab.
2. Run all cells in the notebook.
3. The output of the queries and runtime comparisons will be displayed in the notebook.

## Data

The notebook uses a CSV file of home sales data from an AWS S3 bucket. The data includes information about the price, number of bedrooms, bathrooms, square footage, and other features of homes sold in a particular region.
