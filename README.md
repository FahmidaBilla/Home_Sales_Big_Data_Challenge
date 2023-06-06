# Home_Sales_Big_Data_Challenge


For this challenge, I have used my  knowledge of SparkSQL to determine key metrics about home sales data. Then used Spark to create temporary views, partition the data, cache and uncache a temporary table, and verify that the table has been uncached.

### Following steps were used as per the requirement:

1. Import the necessary PySpark SQL functions for this assignment.

2. Read the home_sales_revised.csv data in the starter code into a Spark DataFrame.

<img width="1053" alt="Fig_1" src="https://github.com/FahmidaBilla/Home_Sales_Big_Data_Challenge/assets/120361200/ca1a35d4-4fe9-406a-ae45-9f469d6b072b">



3. Create a temporary table called home_sales.

4. Answer the following questions using SparkSQL:

- What is the average price for a four-bedroom house sold for each year? Round off answer to two decimal places.

<img width="223" alt="Fig_q_3" src="https://github.com/FahmidaBilla/Home_Sales_Big_Data_Challenge/assets/120361200/7c70208b-3520-47f5-8871-cdb20ff61c5a">



- What is the average price of a home for each year it was built that has three bedrooms and three bathrooms? Round off answer to two decimal places.

<img width="283" alt="Fig_q_4" src="https://github.com/FahmidaBilla/Home_Sales_Big_Data_Challenge/assets/120361200/deb2d4f3-6427-40d5-a03a-98e495837f0c">




- What is the average price of a home for each year that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? Round off answer to two decimal places.

<img width="277" alt="Fig_q_5" src="https://github.com/FahmidaBilla/Home_Sales_Big_Data_Challenge/assets/120361200/91b12d05-e8b5-4c8c-ab03-1abdac85c223">




- What is the "view" rating for homes costing more than or equal to $350,000? Determine the run time for this query, and round off answer to two decimal places.

<img width="361" alt="Fig_q_6_uncached" src="https://github.com/FahmidaBilla/Home_Sales_Big_Data_Challenge/assets/120361200/ddc8b785-f227-4377-9f19-3e36a2ca5511">




5. Cache temporary table home_sales.

6. Check if temporary table is cached.

7. Using the cached data, run the query that filters out the view ratings with an average price of greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.

<img width="376" alt="Fig_q_9_cahced" src="https://github.com/FahmidaBilla/Home_Sales_Big_Data_Challenge/assets/120361200/e42c6b26-09fd-4d10-8f55-3dde9e945f9f">




8. Partition by the "date_built" field on the formatted parquet home sales data.

9. Create a temporary table for the parquet data.

10. Run the query that filters out the view ratings with an average price of greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.

<img width="377" alt="Fig_q_13_parquet" src="https://github.com/FahmidaBilla/Home_Sales_Big_Data_Challenge/assets/120361200/d2f8d88b-32cc-4229-8962-640dc570d700">




11. Uncache the home_sales temporary table.

12. Verify that the home_sales temporary table is uncached using PySpark.


## Result

- The query run time for uncached data is 0.7564346790313721 seconds.

- The query run time for cached data is 0.46768689155578613 seconds.

- The query run time for parquet data is 0.7583417892456055 seconds.


