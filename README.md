# Amazon_Vine_Analysis

Big Data analysis using Google Colab, Pyspark, Postgres/pgAdmin, AWS RDS, and SQL

![204041605-7ec769ed-3454-4fa2-ac8a-338d28b53abb](https://user-images.githubusercontent.com/109055148/213333128-350c574e-fba2-483a-8e97-3b9f050b2e2b.png)

## Overview

For this project, we'll be analyzing Amazon reviews that have been writted by members from the Amazon Vine program, a service the allows both manufactures & publishers to recieve reviews to determine if there are any biaces of their products from Vine team members & Non-Vine members.

Companies paying a fee to Amazon may provide some free products to it's members, are then required to publish a review to help determine if there are biased feedback between Vine members & Non-members. We'll compare or identify 5 start ratings to overall ratings. This exercise, were asked to choose from 50 datasets and extract, transform & load information into a dataframe to complete or analysis.

# Results

There are over 3 million reviews recorded. To drill down and focus on the reviews that will help us with our analysis we'll filter the dataset by:

Count of Total Votes greater or equal to 20.
Percent of Helpful Votes to Total Votes equal or greater than 50%.

![204043885-6ad6cdf2-730f-45d4-be91-f5046b44e85a](https://user-images.githubusercontent.com/109055148/213333211-d9d1e595-4637-4f1d-ad3d-970da0e8ee3b.png)


Results reduced the total number of reviews from 3M to 50.7K. This allowed us to answer the following questions:

1. How many Vine reviews and non-Vine reviews were there?

Vine members made up only 2.1% (1,080) of the reviews whereas the remaining 97.9% were Non-Vine members (49,659).

![204044158-957f49b6-de0a-4006-8f98-04e8e1d586ac](https://user-images.githubusercontent.com/109055148/213333245-f3254057-0282-4314-adf7-e23c9fc5c6bd.png)

![204044256-0e9bac6a-c97a-47eb-8a06-59726d5ac7d7](https://user-images.githubusercontent.com/109055148/213333311-ddd75f67-965b-420a-beb5-48d578a1d367.png)


![204044270-9faac817-d643-42c7-be46-b4195bd3e707](https://user-images.githubusercontent.com/109055148/213333640-9f6accb2-ea3a-41d5-b46a-fa3106c87fca.png)

2.How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

Vine members gave 454 out of 1,080 reviews a 5 star rating.
Non-Vine members gave 23,034 out of 49,659 reviews a 5 star rating.
3.What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

42% of the reviews for Vine members were rated 5 stars.
46.4% of the reviews for Non-Vine members were rated 5 stars.

## Summary

Vine members didn't show bias when rating their products considering that the number of 5-star ratings was 10% less than Non-Vine members (42% vs. 46.4%). We can assume that Vine customers are more critical when submitting their review. However, in order to support this assumption further, we should include all of the data opposed to filtering down to the percentage of helpful vs. total votes, that was used for this analysis. Reviewing the full dataset would give us more information, allowing us to further support our assumption as shown below.


![204048750-6e06b627-53ae-4919-be61-a7959c798464](https://user-images.githubusercontent.com/109055148/213333853-30b3d462-bbf0-4bb7-bc89-7876a8a6f2ff.png)

