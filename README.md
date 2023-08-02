#### "Data-driven insights and performance optimization using SparkSQL for key metrics analysis and efficient data management in home sales data."

## Background

The real estate industry generates vast amounts of data, and analyzing this data can provide valuable insights into housing market trends and patterns. SparkSQL, a component of Apache Spark, enables efficient processing and analysis of structured and semi-structured data using SQL-like queries. In this project, we utilize SparkSQL to analyze home sales data, gaining key metrics and answering specific questions about the dataset. By leveraging the power of Spark, we can extract meaningful information to inform decision-making in the real estate domain.

## Objectives

1. Utilize SparkSQL to analyze and derive key metrics from home sales data.
2. Determine the average price for four-bedroom houses sold each year.
3. Calculate the average price of homes for each year they were built, considering three bedrooms and three bathrooms.
4. Find the average price of homes for each year, considering three bedrooms, three bathrooms, two floors, and a size of at least 2,000 square feet.
5. Identify the "view" rating for homes with a price greater than or equal to $350,000 and measure the query's runtime.
6. Cache the temporary table "home_sales" to optimize query performance.
7. Verify that the "home_sales" temporary table is successfully cached.
8. Compare the runtime of the query filtering view ratings with prices greater than or equal to $350,000 between cached and uncached data.
9. Partition the formatted parquet home sales data by the "date_built" field.
10. Create a temporary table for the parquet data to enable further analysis.
11. Measure the runtime of the query filtering view ratings with prices greater than or equal to $350,000 on the parquet data and compare it with the uncached runtime.
12. Uncache the temporary table "home_sales."
13. Verify the successful uncaching of the "home_sales" temporary table using PySpark.
14. Share the Home_Sales.ipynb file by uploading it to the "Home_Sales" GitHub repository.

## Methods
1. Import necessary PySpark SQL functions.
2. Read the provided home_sales_revised.csv data into a Spark DataFrame.
3. Create a temporary table named "home_sales" to perform SparkSQL queries on the dataset.
4. Execute various SparkSQL queries to obtain the required metrics and answers.
5. Cache the "home_sales" temporary table to improve query performance.
6. Verify the successful caching of the temporary table.
7. Re-run the query on the cached data to compare the runtime with the uncached query.
8. Partition the formatted parquet home sales data by the "date_built" field.
9. Create a temporary table for the parquet data to enable further analysis.
10. Execute the query on the parquet data and compare the runtime with the uncached query.
11. Uncache the "home_sales" temporary table.
12. Verify the successful uncaching of the temporary table using PySpark.
13. Upload the Home_Sales.ipynb file to the "Home_Sales" GitHub repository for sharing and reference.

## Results

![home_sales](https://user-images.githubusercontent.com/114210481/231291277-20f52e84-fca7-4dcc-8f62-36f3342c4b91.jpg)

- What is the average price for a four-bedroom house sold for each year? Round off your answer to two decimal places.

![avgprice_4bed](https://user-images.githubusercontent.com/114210481/231291327-16fe8377-bde4-424b-b7ad-5cf6bb19f644.jpg)

- What is the average price of a home for each year it was built that has three bedrooms and three bathrooms? Round off your answer to two decimal places.

![avgprice_3bed_3bath](https://user-images.githubusercontent.com/114210481/231291355-a1a3cecc-f080-41a3-8454-4bfa13badd25.jpg)

- What is the average price of a home for each year that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? Round off your answer to two decimal places.

![avgprice_3bed_3bath_2fl](https://user-images.githubusercontent.com/114210481/231291406-136d2eec-5aee-49a5-8b05-f049ab055bcf.jpg)

- What is the "view" rating for homes costing more than or equal to $350,000? Determine the run time for this query, and round off your answer to two decimal places.

![avgprice_view](https://user-images.githubusercontent.com/114210481/231291446-e4eb42c7-c68a-48de-ab71-7fb75bc6dd83.jpg)

Run time : 0.2731211185455322 seconds

![avgprice_view_cached](https://user-images.githubusercontent.com/114210481/231291474-d151ea7d-d575-4202-943e-2bc7c0bd46a8.jpg)

Run time : 0.18812322616577148 seconds

![avgprice_view_parquet](https://user-images.githubusercontent.com/114210481/231291504-77bc936c-b78d-4108-bb03-c63635b32ddd.jpg)

Run time : 0.18667101860046387 seconds



### Sources:

https://courses.bootcampspot.com/courses/2799/assignments/42933?module_item_id=804089

https://spark.apache.org/docs/latest/api/python/getting_started/index.html
