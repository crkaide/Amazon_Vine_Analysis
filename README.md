# Amazon Vine Analysis
_source data: https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Apparel_v1_00.tsv.gz_

## Overview of the analysis
The primary purpose of this analysis is to inform the decisions of manufacturers and publishers with regard to the value of Amazon's paid review program, Vine.  The working hypothesis of this analysis is that paying Vine reviewers creates a positive bias in favor of the company providing the product.  Analysis was primarily done using a Google colab notebook and Python.

## Results table
![del_3_a.png](https://github.com/crkaide/Amazon_Vine_Analysis/blob/main/Images/del_3_a.png?raw=true)

1. There were 33 total vine reviews and 45,388 non-Vine reviews.
2. There were 15 5-star Vine ratings and 23,733 5-star non-Vine ratings.
3. 45% of Vine reviews were 5-star.  52% of non-Vine reviews were 5-star.

## Summary
The results of this analysis force us to fail our working hypothesis and conclude that there is currently no evidence for a positive bias in the company's favor when a review is written by a paid participant in the Vine program (paid 45% 5-star vs. unpaid 52% 5-star.

## Add'l analysis
There are two primary limitations to this analysis:

1. The scope is limited to 5-star reviews, while not all positive reviews are necessarily 5-star
2. Analysis does not take textual input into account

I recommend additional analysis that buckets all reviews as follows: positive = 4 & 5 star, neutral = 3 star, negative = 2 & 1 star.  Stacked bar graphs of paid vs. unpaid with this categorization will more comprehensively support failing the hypothesis (if failing it holds up under this add'l analysis).  

While reviews are assigned a rating, sentiment analysis and keyword identification of the review text would likely add great value to this report.
