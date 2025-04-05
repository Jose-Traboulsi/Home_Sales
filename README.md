# Home_Sales

🏡 Home Sales Data Analysis with PySpark

Overview
This project leverages Apache Spark and PySpark SQL to analyze home sales data stored in CSV and Parquet formats. The dataset includes various features such as number of bedrooms, bathrooms, square footage, year built, and view ratings. The goal is to use SparkSQL to extract insights efficiently and optimize query performance using caching and partitioning techniques.

📂 Files Included
Home_Sales.ipynb – Final Jupyter Notebook with all tasks completed and code executed.
home_sales_revised.csv – Source data file (loaded from an AWS S3 bucket).

🔍 Key Tasks Completed
Initial Setup
Renamed starter notebook to Home_Sales.ipynb.
Imported necessary PySpark SQL functions.

Data Ingestion
Loaded home_sales_revised.csv from an AWS S3 bucket into a Spark DataFrame.
Created a temporary table named home_sales.

Data Analysis Using SparkSQL
Calculated average price of 4-bedroom homes sold each year.
Found average home price per year built for homes with 3 beds and 3 baths.
Computed average price by year built for homes with 3 beds, 3 baths, 2 floors, and ≥ 2000 sqft.
Calculated average price by 'view' rating for homes with an average price ≥ $350,000, and measured runtime.

Optimization Techniques
Cached the home_sales temporary table.
Verified cache status and re-ran performance-sensitive query to compare runtimes (cached vs. uncached).
Saved formatted data to Parquet, partitioned by date_built.
Created a temporary table on partitioned data and re-ran the performance-sensitive query.
Uncached and verified the uncaching of the home_sales table.

⚙️ Technologies Used
Python
PySpark (Spark SQL)
Jupyter Notebook

AWS S3
Parquet Format

