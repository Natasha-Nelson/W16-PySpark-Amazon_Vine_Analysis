# W16-PySpark-Amazon_Vine_Analysis

## Overview:
The purpose of this analysis was to explore the potential impact Amazon's Vine program has on review scores. For this analysis, I worked with a dataset from the publically available data listed below:
https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt --> https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Tools_v1_00.tsv.gz

In this project, I worked with AWS RDS, AWS S3, PgAdmin/SQL, and PySpark/Google Colab. Using these tools, I explored the dataset above to understand whether participation in the vine program positive skews reviews.

## Results: 
![Figure_Vine_Analysis](https://user-images.githubusercontent.com/81983110/128654116-001ad3a5-a53a-48b8-95ed-af6d33f41df4.png)

1. How many Vine reviews and non-Vine reviews were there? As part of the set up for this experiment, we choose to focus on reviews with over 20 votes and over 50% 'helpful' votes, aka the "most helpful" reviews There were 29,720 total helpful reviews, 29,452 unpaid reviews and 268 Vine reviews. 
2. How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?  There were 13,817 helpful reviews, 149 helpful Vine reviews and 13,668 helpful unpaid reviews. 
3. What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars? 55% of unpaid helpful reviews were five star reviews, whereas 46% of Vine reviews are five stars. 

**Figures Representing Review Databases**
Summary: In your summary, state if there is any positivity bias for reviews in the Vine program. Use the results of your analysis to support your statement. Then, provide one additional analysis that you could do with the dataset to support your statement.
