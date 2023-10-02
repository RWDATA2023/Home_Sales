# Home_Sales
This project dives into analyzing home sales data using SparkSQL. By setting up a robust environment within Google Colab, we explore key metrics associated with home sales. Starting from ingesting data into a Spark DataFrame, the journey involves creating temporary tables, running a series of intricate queries ranging from understanding average prices based on various conditions to assessing the "view" ratings of homes. Not stopping there, we delve into performance optimization by caching tables and experimenting with the Parquet format. All the findings, code, and detailed steps are neatly documented in the Home_Sales.ipynb notebook available in the Home_Sales GitHub repository.

Setting Up
After importing the necessary libraries and getting everything ready in Colab, I started up a SparkSQL session.

Getting the Data
I grabbed the data from an AWS S3 bucket, turned it into a DataFrame, and then set up a temporary table. This table made it easier to run SQL-like queries.

What I Found
Using SparkSQL, I ran several queries to figure out:

How home prices have changed over time.
The price differences based on factors like number of bedrooms and bathrooms.
Speeding Up Queries
I also played around with caching to speed up the queries. After caching the table, I found that the same queries ran faster, which was pretty cool to see.

Trying Out Parquet
I heard about Parquet, a format that's optimized for big data. So, I gave it a shot. Converted the data to Parquet, ran the queries again, and found that while Parquet did speed things up, cached data was still the fastest.

Wrapping Up
In the end, I uncached the data and wrapped up the analysis. Oh, and a quick tip: If you're running this in Colab and run into issues with findspark, try switching the Spark version to 3.5.0.

Takeaway
This project was a great way to dive deep into data using SparkSQL, learn about performance optimization, and get hands-on with Google Colab. If you're into data and want to explore big datasets, SparkSQL is definitely worth a look.