# Amazon_Vine_Analysis

## Overview 

Using knowledge of the cloud ETL process, we create an AWS RDS database with tables in pgAdmin, pick a dataset from the Amazon Review datasets (we chose: https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Wireless_v1_00.tsv.gz), and extract the dataset into a DataFrame. We transform the DataFrame into four separate DataFrames that match the table schema in pgAdmin. Then, upload the transformed data into the appropriate tables.

Also, using knowledge of PySpark, Pandas, or SQL, we determine if there is any bias towards reviews that were written as part of the Vine program. For this analysis, we determine if having a paid Vine review makes a difference in the percentage of 5-star reviews.

## Results:

How many Vine reviews and non-Vine reviews were there?

- There were 613 Vine reviews and 64,968 non-Vine reviews.

How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

- There were 222 Vine reviews with 5 stars and 30,543 non-Vine reviews with 5 stars.

What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

- 36%% of Vine reviews were 5 stars and 47% of non-Vine reviews were 5 stars.

### Images of DataFrames showing percentage of Vine/non-Vine reviews that were 5 stars

![percentage_5_star_vine.png](https://github.com/alexhuynh0530/Amazon_Vine_Analysis/blob/main/percentage_5_star_vine.png)

## Summary: State if there is any positivity bias for reviews in the Vine program. Use the results of your analysis to support your statement. Then, provide one additional analysis that you could do with the dataset to support your statement.

As seen from the results of the data, there is not a positivity bias for reviews in the Vine program. You see this because non_Vine reviews had a higher percentage of 5 star reviews versus the percentage of Vine reviews that were 5 stars.

You could also add 4 star reviews and check the percentage of 4-5 star reviews for Vine versus non_Vine reviews.
