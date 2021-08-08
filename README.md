# Amazon_Vine_Analysis

## Overview 
The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies can pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review. The purpose of this analysis is to analyze whether or not there is any favorable bias towards products that participate in vine program.  Using Amazon's vast database of product reviews, we can use PySpark to perform an ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into a PostgreSQL database. From there, we can extract and analyze the data in a Jupyter Notebook. Amazon provides [a huge list of open datasets](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt) that showcase reviews across all sorts of product categories. For this analysis, the dataset chosen was Musical Instruments. 

