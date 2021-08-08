# Amazon_Vine_Analysis

## Overview 
The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies can pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review. The purpose of this analysis is to analyze whether or not there is any favorable bias towards products that participate in vine program.  Using Amazon's vast database of product reviews, we can use PySpark to perform an ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into a PostgreSQL database. From there, we can extract and analyze the data in a Jupyter Notebook. Amazon provides [a huge list of open datasets](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt) that showcase reviews across all sorts of product categories. For this analysis, the dataset chosen was Musical Instruments. 

## Results 

[Summary Table of Results](https://github.com/matthewprice-github/Amazon_Vine_Analysis/blob/main/Amazon_Vine_Analysis/Vine_Analysis_Summary.PNG)

The volume of reviews were also skewed heavily towards the non-Vine group, with over 13.5K total reviews compared to only 59 total reviews for Vine. This volume differential continued proportionally to fivestar reviews, of which there were 7.7K five star reviews in the non-Vine products, and only 34 five star Vine reviews. This leads to a five star review percentage of 56.96% and 57.63% of Non-Vine and Vine reviews, respectively. 


## Summary

Given these results, there does not appear to be significant bias in five star reivews given to products in the Vine program, at least in the musical instrument category. While Vine reviews do have a nominally higher percentage of five star reviews, the difference is within 1 percentage point of the non-Vine average. It would be interesting to see if this same pattern holds for other Amazon product categories, bias could be present for other types of products. Another interesting thing would be to see how the five star percentages vary across different product cateogires. It is a universal phenomenon that over half of reviews deemed "helpful" are five stars? Amazon's datasets are super large so the possibilities for further analysis are vast. 




