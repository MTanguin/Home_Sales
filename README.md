# Home_Sales

## OBJECTIVES

- Use SparkSQL to determine key metrics about home sales data. 
- Use Spark to create temporary views, partition the data, cache and uncache a temporary table, and verify that the table has been uncached.

## INSTRUCTIONS


1. Rename the Home_Sales_starter_code.ipynb file as Home_Sales.ipynb.

2. Import the necessary PySpark SQL functions for this assignment.

3. Read the home_sales_revised.csv data in the starter code into a Spark DataFrame.

![Alt text](Starter_Code/Images/home_sales.jpg)


4. Create a temporary table called home_sales.

![Alt text](Starter_Code/Images/home_sales.jpg)


5. Answer the following questions using SparkSQL:

- What is the average price for a four-bedroom house sold for each year? Round off your answer to two decimal places.


![Alt text](Starter_Code/Images/avgprice_4bed.jpg)


- What is the average price of a home for each year it was built that has three bedrooms and three bathrooms? Round off your answer to two decimal places.

![Alt text](Starter_Code/Images/avgprice_3bed_3bath.jpg)


- What is the average price of a home for each year that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? Round off your answer to two decimal places.

![Alt text](Starter_Code/Images/avgprice_3bed_3bath_2fl.jpg)

- What is the "view" rating for homes costing more than or equal to $350,000? Determine the run time for this query, and round off your answer to two decimal places.

![Alt text](Starter_Code/Images/avgprice_view.jpg)

Run time : 0.2731211185455322 seconds

6. Cache your temporary table home_sales.

7. Check if your temporary table is cached.

8. Using the cached data, run the query that filters out the view ratings with an average price of greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.

![Alt text](Starter_Code/Images/avgprice_view_cached.jpg)

Run time : 0.18812322616577148 seconds

9. Partition by the "date_built" field on the formatted parquet home sales data.

10. Create a temporary table for the parquet data.

11. Run the query that filters out the view ratings with an average price of greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.

![Alt text](Starter_Code/Images/avgprice_view_parquet.jpg)

Run time : 0.18667101860046387 seconds

12. Uncache the home_sales temporary table.

13. Verify that the home_sales temporary table is uncached using PySpark.

14. Download your Home_Sales.ipynb file and upload it into your "Home_Sales" GitHub repository.
