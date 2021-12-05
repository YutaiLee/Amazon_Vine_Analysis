# Amazon_Vine_Analysis
## Overview of the project
This project analyzes Amazon Vine program and determines if there is a bias toward favorable reviews from Vine members. The analysis uses PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, load the transformed data into pgAdmin and calculate different metrics. We focused on the US reviews for shoes.
### Results
1. How many Vine reviews and non-Vine reviews were there?

Vine members accounted for only 0.08% (22) of the reviews, while the remaining non-Vine members accounted for 99.92%.

![image](https://github.com/YutaiLee/Amazon_Vine_Analysis/blob/main/images/rating_total_df.png)

![image](https://github.com/YutaiLee/Amazon_Vine_Analysis/blob/main/images/paid_df.png)

![image](https://github.com/YutaiLee/Amazon_Vine_Analysis/blob/main/images/non_paid_df.png)

2. How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
  * Vine members gave 13 out of 22 reviews a 5-star rating.
  * Non-Vine members gave 14476 out of 26987 reviews a 5-star rating.
3. What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
  * 59.09% of the reviews for Vine members were rated 5 stars.
  * 53.64% of the reviews for Non-Vine members were rated 5 stars.
### Summary
59.09% of the reviews in the Vine program were 5 stars reviews whereas the percentage in the non-Vine reviews is only 53.64%. This describes a positivity bias for reviews in the Vine program.
Additionally we could analyse the statistical distribution (mean, median and mode) of the star rating for the Vine and non-Vine reviews.
