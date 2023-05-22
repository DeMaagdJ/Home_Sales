# Home_Sales
Module 22 HW Assignment

In this challenge, you'll use your knowledge of SparkSQL to determine key metrics about home sales data. Then you'll use Spark to create temporary views, partition the data, cache and uncache a temporary table, and verify that the table has been uncached.


## Instructions

1. Rename the Home_Sales_starter_code.ipynb file as Home_Sales.ipynb

2. Import the necessary PySpark SQL functions for this assignment.
3. Read the home_sales_revised.csv data in the starter code into a Spark DataFrame.

/var/folders/xw/z2rhr7zj1kvg3zdq580t0_340000gp/T/TemporaryItems/NSIRD_screencaptureui_1nbsrY/Screenshot 2023-05-22 at 10.23.40 AM.pngnb.

4. Create a temporary table called home_sales.

/var/folders/xw/z2rhr7zj1kvg3zdq580t0_340000gp/T/TemporaryItems/NSIRD_screencaptureui_IlJqAK/Screenshot 2023-05-22 at 10.24.58 AM.png

5. Answer the following questions using SparkSQL:
* What is the average price for a four-bedroom house sold for each year? Round off your answer to two decimal places.

/var/folders/xw/z2rhr7zj1kvg3zdq580t0_340000gp/T/TemporaryItems/NSIRD_screencaptureui_ApMcTs/Screenshot 2023-05-22 at 10.26.04 AM.png

* What is the average price of a home for each year it was built that has three bedrooms and three bathrooms? Round off your answer to two decimal places.

/var/folders/xw/z2rhr7zj1kvg3zdq580t0_340000gp/T/TemporaryItems/NSIRD_screencaptureui_w3DBqs/Screenshot 2023-05-22 at 10.26.33 AM.png

* What is the average price of a home for each year that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? Round off your answer to two decimal places.

/var/folders/xw/z2rhr7zj1kvg3zdq580t0_340000gp/T/TemporaryItems/NSIRD_screencaptureui_VPgXw0/Screenshot 2023-05-22 at 10.27.47 AM.png

* What is the "view" rating for homes costing more than or equal to $350,000? Determine the run time for this query, and round off your answer to two decimal 

/var/folders/xw/z2rhr7zj1kvg3zdq580t0_340000gp/T/TemporaryItems/NSIRD_screencaptureui_nnUQZy/Screenshot 2023-05-22 at 10.28.47 AM.pngplaces.

6. Cache your temporary table home_sales.

/var/folders/xw/z2rhr7zj1kvg3zdq580t0_340000gp/T/TemporaryItems/NSIRD_screencaptureui_YHaL9Q/Screenshot 2023-05-22 at 10.30.27 AM.png

7. Check if your temporary table is cached.

/var/folders/xw/z2rhr7zj1kvg3zdq580t0_340000gp/T/TemporaryItems/NSIRD_screencaptureui_qM3N7v/Screenshot 2023-05-22 at 10.31.08 AM.png

8. Using the cached data, run the query that filters out the view ratings with an average price of greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.

/var/folders/xw/z2rhr7zj1kvg3zdq580t0_340000gp/T/TemporaryItems/NSIRD_screencaptureui_OjLhe3/Screenshot 2023-05-22 at 10.31.54 AM.png

9. Partition by the "date_built" field on the formatted parquet home sales data.

/var/folders/xw/z2rhr7zj1kvg3zdq580t0_340000gp/T/TemporaryItems/NSIRD_screencaptureui_DRXbmb/Screenshot 2023-05-22 at 10.32.26 AM.png

10. Create a temporary table for the parquet data.

/var/folders/xw/z2rhr7zj1kvg3zdq580t0_340000gp/T/TemporaryItems/NSIRD_screencaptureui_0mVEYo/Screenshot 2023-05-22 at 10.32.57 AM.png

11. Run the query that filters out the view ratings with an average price of greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.

/var/folders/xw/z2rhr7zj1kvg3zdq580t0_340000gp/T/TemporaryItems/NSIRD_screencaptureui_n9zU7W/Screenshot 2023-05-22 at 10.33.38 AM.png

12. Uncache the home_sales temporary table.

/var/folders/xw/z2rhr7zj1kvg3zdq580t0_340000gp/T/TemporaryItems/NSIRD_screencaptureui_fmp5vW/Screenshot 2023-05-22 at 10.34.15 AM.png

13. Verify that the home_sales temporary table is uncached using PySpark.

/var/folders/xw/z2rhr7zj1kvg3zdq580t0_340000gp/T/TemporaryItems/NSIRD_screencaptureui_5MD30P/Screenshot 2023-05-22 at 10.34.36 AM.png

14. Download your Home_Sales.ipynb file and upload it into your "Home_Sales" GitHub repository.