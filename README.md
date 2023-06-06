# Module-22-challenge
Home_Sales
This Python script uses PySpark to analyze home sales data. It reads data from an AWS S3 bucket, converts the data to a Spark DataFrame, creates temporary views of the data, caches the views, and performs various SQL queries on the cached data.

The script requires Spark and Java to be installed. It downloads and installs the latest version of Spark 3.x, installs Java, and sets environment variables. It also imports the necessary packages, including pandas and findspark.

The script performs the following queries on the home sales data:

Read in the AWS S3 bucket into a DataFrame.
Create a temporary view of the DataFrame.
What is the average price for a four-bedroom house sold in each year rounded to two decimal places?
What is the average price of a home for each year the home was built that have 3 bedrooms and 3 bathrooms rounded to two decimal places?
What is the average price of a home for each year built that have 3 bedrooms, 3 bathrooms, with two floors, and are greater than or equal to 2,000 square feet rounded to two decimal places?
What is the "view" rating for the average price of a home, rounded to two decimal places, where the homes are greater than or equal to $350,000? Although this is a small dataset, determine the run time for this query.
Cache the temporary table home_sales.
Check if the table is cached.
Using the cached data, run the query that filters out the view ratings with average price greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.
Partition by the "date_built" field on the formatted parquet home sales data.
Read the parquet formatted data.
Create a temporary table for the parquet data.
The script saves the cached dataframe as partitioned parquet.

To run the script, specify the latest version of Spark 3.x from http://www.apache.org/dist/spark/ and enter it as the spark_version. Then run the script in a Python environment that has PySpark and the required packages installed.
