# Amazon Vine Analysis

## Overview
For this project, we utilized Google Colab Notebooks as a tool to parse through Amazon review data for shoes. The purpose of this project was to determine if there is any bias towards reviews that were written as part of the Vine program. We focused on a comparison of paid and unpaid Vine reviews.

## Results
We began using SparkPy in a Google Colab Notebook. We brought in the Vine Reviews, and filtered down to a new dataframe wheretotal votes were greater than 20, and helpful votes divided by total votes were over 50%.

![helpful_df](https://github.com/bessobrien/Amazon_Vine_Analysis/blob/main/Resources/helpful_df.png)

We then created two separate dataframes: one with all reviews written as part of the Vine program, and one where all reviews were not written as part of the Vine program.

We then did some simple math for each set:
1. Total Number of Reviews
2. Total Number of 5-Star Reviews
3. Percentage of 5-Star Reviews

For our "YES" Vine reviews, we saw that we had 20 total reviews, 12 5-star reviews, for a percentage of 60% of 5-star reviews.
![yes_results](https://github.com/bessobrien/Amazon_Vine_Analysis/blob/main/Resources/yes_results.png)

For our "NO" non-Vine reviews, we saw that we had 25,116 total reviews, 13,479 5-star reviews, for a percetage of 53.7% of 5-star reviews.
![no_results](https://github.com/bessobrien/Amazon_Vine_Analysis/blob/main/Resources/no_results.png)

## Summary

In conclusion, we believe that there is some positivity bias for reviews in the Vine program. Being paid adds some incentive to leave a more positive review. To further research, I recommend an additional analysis that would pull the number of 1 and 2-star reviews as well. This would provide further data points to bolster our initial conclusion.
