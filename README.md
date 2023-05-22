# Home_Sales
Module 22 HW Assignment

In this challenge, you'll use your knowledge of SparkSQL to determine key metrics about home sales data. Then you'll use Spark to create temporary views, partition the data, cache and uncache a temporary table, and verify that the table has been uncached.


## Instructions

1. Rename the Home_Sales_starter_code.ipynb file as Home_Sales.ipynb

2. Import the necessary PySpark SQL functions for this assignment.
3. Read the home_sales_revised.csv data in the starter code into a Spark DataFrame.

<img width="892" alt="Screenshot 2023-05-22 at 10 46 18 AM" src="https://github.com/DeMaagdJ/Home_Sales/assets/119906575/ced4ca7c-f802-4aae-8744-738b098b5275">


4. Create a temporary table called home_sales.

<img width="401" alt="Screenshot 2023-05-22 at 10 46 44 AM" src="https://github.com/DeMaagdJ/Home_Sales/assets/119906575/ecf087f3-62bc-4cfc-bd35-0573fd1d1154">


5. Answer the following questions using SparkSQL:
* What is the average price for a four-bedroom house sold for each year? Round off your answer to two decimal places.

<img width="823" alt="Screenshot 2023-05-22 at 10 47 07 AM" src="https://github.com/DeMaagdJ/Home_Sales/assets/119906575/f8d0ecff-c5f9-4cfa-89b1-0fd8e65dad68">


* What is the average price of a home for each year it was built that has three bedrooms and three bathrooms? Round off your answer to two decimal places.

<img width="1095" alt="Screenshot 2023-05-22 at 10 47 24 AM" src="https://github.com/DeMaagdJ/Home_Sales/assets/119906575/6bf55322-ab45-4a02-a4b7-3233815f0ca5">

* What is the average price of a home for each year that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? Round off your answer to two decimal places.

<img width="1123" alt="Screenshot 2023-05-22 at 1 51 43 PM" src="https://github.com/DeMaagdJ/Home_Sales/assets/119906575/89757811-3797-43e7-806a-b84ec540c78d">


* What is the "view" rating for homes costing more than or equal to $350,000? Determine the run time for this query, and round off your answer to two decimal places.

<img width="1049" alt="Screenshot 2023-05-22 at 1 52 43 PM" src="https://github.com/DeMaagdJ/Home_Sales/assets/119906575/79c4f149-1a98-4e72-af15-d29ac4ac53b0">

6. Cache your temporary table home_sales.

<img width="586" alt="Screenshot 2023-05-22 at 10 50 20 AM" src="https://github.com/DeMaagdJ/Home_Sales/assets/119906575/d6dea33d-0d9c-4dc5-a0d3-c7a9b705ba90">

7. Check if your temporary table is cached.

<img width="323" alt="Screenshot 2023-05-22 at 10 50 47 AM" src="https://github.com/DeMaagdJ/Home_Sales/assets/119906575/d2bbf9d1-9df2-41d2-b608-777862570c01">

8. Using the cached data, run the query that filters out the view ratings with an average price of greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.

<img width="931" alt="Screenshot 2023-05-22 at 1 53 59 PM" src="https://github.com/DeMaagdJ/Home_Sales/assets/119906575/a57629f3-7e77-464c-9628-aa4a9d73a1b5">

9. Partition by the "date_built" field on the formatted parquet home sales data.

<img width="658" alt="Screenshot 2023-05-22 at 10 52 04 AM" src="https://github.com/DeMaagdJ/Home_Sales/assets/119906575/e0fb5962-873a-4619-be14-06366218e970">

10. Create a temporary table for the parquet data.

<img width="463" alt="Screenshot 2023-05-22 at 10 52 26 AM" src="https://github.com/DeMaagdJ/Home_Sales/assets/119906575/fa64ee2c-4862-47f2-805f-98f8ae4b71cb">

11. Run the query that filters out the view ratings with an average price of greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.

<img width="998" alt="Screenshot 2023-05-22 at 1 55 16 PM" src="https://github.com/DeMaagdJ/Home_Sales/assets/119906575/2946361c-4451-430e-95fd-c5f736f56c26">

12. Uncache the home_sales temporary table.

<img width="385" alt="Screenshot 2023-05-22 at 10 54 16 AM" src="https://github.com/DeMaagdJ/Home_Sales/assets/119906575/43ba72e7-87ca-45a4-8b1a-7c4754fde8b1">

13. Verify that the home_sales temporary table is uncached using PySpark.

<img width="547" alt="Screenshot 2023-05-22 at 10 54 40 AM" src="https://github.com/DeMaagdJ/Home_Sales/assets/119906575/0737ab3a-1c86-4b6e-8a17-9565a9142bf6">

14. Download your Home_Sales.ipynb file and upload it into your "Home_Sales" GitHub repository.

## Results

After querying the uncached view we started at a run time of 6.1 seconds.  After caching the SQL table I was able to reduce the run time down to 5.5 seconds.  After partitioning the parquet format I was able to recude the run time to view the SQL query to 4.1 seconds.  Ultimately caching data speeds up performance and increase the efficiency when analyzing SQL queries.
