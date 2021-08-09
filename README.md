# W16-PySpark-Amazon_Vine_Analysis

## Overview:
The purpose of this analysis was to explore the potential impact Amazon's Vine program has on review scores. For this analysis, I worked with a dataset from the publically available data listed below:
https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt --> https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Tools_v1_00.tsv.gz

In this project, I worked with AWS RDS, AWS S3, PgAdmin/SQL, and PySpark/Google Colab. Using these tools, I explored the dataset above to understand whether participation in the vine program positive skews reviews.

## Results: 
### Summary Figure
![Figure_Vine_Analysis](https://user-images.githubusercontent.com/81983110/128654116-001ad3a5-a53a-48b8-95ed-af6d33f41df4.png)

1. How many Vine reviews and non-Vine reviews were there? As part of the set up for this experiment, we choose to focus on reviews with over 20 votes and over 50% 'helpful' votes, aka the "most helpful" reviews There were 29,720 total helpful reviews, 29,452 unpaid reviews and 268 Vine reviews. 
2. How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?  There were 13,817 helpful reviews, 149 helpful Vine reviews and 13,668 helpful unpaid reviews. 
3. What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars? 55% of unpaid helpful reviews were five star reviews, whereas 46% of Vine reviews are five stars. 

### Figures Representing Review Databases**
#### Full "Helpful" Review DF

![Helpful_DF](https://user-images.githubusercontent.com/81983110/128654610-203279d6-ac6f-41d5-8431-3d2910256dfa.png)

#### Unpaid "Helpful" Review DF

![Unpaid_DF](https://user-images.githubusercontent.com/81983110/128654611-685326ce-6627-4721-a101-4e46d726a0b6.png)

#### Vine "Helpful" Review DF

![Vine_DF](https://user-images.githubusercontent.com/81983110/128654613-43514566-e6be-4dce-97a8-d34dd03163f7.png)

## Summary:
Based on my results, there is no positivity bias for reviews in the Vine program. We noticed that the percentage of 5 star Vine reviews is lower than the percentage of unpaid reviews. However, it is also worth noting that the percentage of Vine reviews within the 5 star group is higher than than the non-5 star group (1.08% to 0.90%). Further analysis could be done to:
1. Interpret the statistical significance of our results
2. Breakdown the percentage of reviews for other star-counts (eg. 4 stars or 3 stars)
3. Compare these results across other Vine datasets
4. Examining results on 'unhelpful' reviews or reviews with less votes

The number of Vine reviews relative to the overall number of reviews is quite low and unlikely to impact to the overall average number of stars. However, to truly validate these results, a greater sample size would be a great place to start. 
