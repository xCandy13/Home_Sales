# Home_Sales
Home_Sales_code.ipynb contains the Python code to read the home_sales_revised.csv into a Spark DataFrame. It then answers four analysis questions using SparkSQL queries:
* What is the average price for a four-bedroom house sold for each year?
* What is the average price of a home for each year it was built that has three bedrooms and three bathrooms?
* What is the average price of a home for each year that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet?
* What is the "view" rating for homes costing more than or equal to $350,000?
The code then caches the table and runs the "view" rating query again, and parquet-partitions the data and runs the "view" rating query a third time, comparing the runtime for each iteration.
Finally, the code uncaches the table.