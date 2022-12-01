# Big-Data-ETL
------------------------------
Many of Amazon's shoppers depend on product reviews to make a purchase. Amazon makes these datasets publicly available. They are quite large and can exceed the capacity of local machines. One dataset alone contains over 1.5 million rows; with over 40 datasets, data analysis can be very demanding on the average local computer. My first goal will be to perform the ETL process completely in the cloud and upload a DataFrame to an RDS instance. The second goal will be to use PySpark or SQL to perform a statistical analysis of selected data.

I will be extracting two Amazon customer review datasets, and transform each dataset into four DataFrames, and load the DataFrames into an RDS instance.

Part 1:
* Explore the Amazon Reviews Links to an external site.datasets and pick two datasets to perform ETL.
* Extract the data by reading in each dataset using the correct header and sep parameters, and get the number of rows in the dataset.
* Create the "review_id_df" DataFrame with the appropriate columns and data types.
* Create the "products_df" DataFrame that drops the duplicates in the "product_id" and "product_title columns.
* Create the "customers_df" DataFrame that groups the data on the "customer_id" by the number of times a customer reviewed a product.
* Create the "vine_df" DataFrame that has the "review_id", "star_rating", "helpful_votes", "total_votes", and "vine" columns.
* Export each DataFrame into the RDS instance to create four tables for each dataset.