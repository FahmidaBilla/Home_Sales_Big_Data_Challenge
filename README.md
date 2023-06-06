# Home_Sales_Big_Data_Challenge

For this challenge, I have used my  knowledge of SparkSQL to determine key metrics about home sales data. Then used Spark to create temporary views, partition the data, cache and uncache a temporary table, and verify that the table has been uncached.

### Following steps were used as per the requirement:

1. Import the necessary PySpark SQL functions for this assignment.

2. Read the home_sales_revised.csv data in the starter code into a Spark DataFrame.



3. Create a temporary table called home_sales.

4. Answer the following questions using SparkSQL:

    - What is the average price for a four-bedroom house sold for each year? Round off answer to two decimal places.



    - What is the average price of a home for each year it was built that has three bedrooms and three bathrooms? Round off answer to two decimal places.



    - What is the average price of a home for each year that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? Round off answer to two decimal places.



    - What is the "view" rating for homes costing more than or equal to $350,000? Determine the run time for this query, and round off answer to two decimal places.




5. Cache temporary table home_sales.

6. Check if temporary table is cached.

7. Using the cached data, run the query that filters out the view ratings with an average price of greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.





8. Partition by the "date_built" field on the formatted parquet home sales data.

9. Create a temporary table for the parquet data.

10. Run the query that filters out the view ratings with an average price of greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.




11. Uncache the home_sales temporary table.

12. Verify that the home_sales temporary table is uncached using PySpark.




## Result

- The query run time for uncached data is 0.7564346790313721 seconds.

- The query run time for cached data is 0.46768689155578613 seconds.

- The query run time for parquet data is 0.7583417892456055 seconds.


