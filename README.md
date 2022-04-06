# Amazon_Vine_Analysis

## Overview 

For the purpose of this project, I picked the Pet product reviews from Amazon and used the Pyspark to perform the ETL process by extracting the data, transforming the data and connecting to the database that we generated through the AWS webserver and loading the transformed data into pgAdmin.  The whole goal of this project was to analyze the information and determine if there is any bias toward favorable reviews from Vine members in your dataset and then, write a summary of the analysis for Jennifer to submit to the SellBy stakeholders.
My Dataset: Pet Products - https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Pet_Products_v1_00.tsv.gz

## Results

### How many vine reviews?

![total-vine-reviews](https://github.com/backwater-graphics/Amazon_Vine_Analysis/blob/main/Resources/total-vine-reviews.jpg)
---

### How many non-vine reviews?

![total-nonvine-reviews](https://github.com/backwater-graphics/Amazon_Vine_Analysis/blob/main/Resources/total-nonvine-reviews.jpg)
---

### How many Vine reviews were 5 stars? 

![five-star-vine-review](https://github.com/backwater-graphics/Amazon_Vine_Analysis/blob/main/Resources/five-star-nonvine-review.jpg)
---

### How many non-Vine reviews were 5 stars?

![five-star-nonvine-review](https://github.com/backwater-graphics/Amazon_Vine_Analysis/blob/main/Resources/five-star-vine-review.jpg)
---

### What percentage of Vine reviews were 5 stars? 

![percentage-paid-review](https://github.com/backwater-graphics/Amazon_Vine_Analysis/blob/main/Resources/percentage-paid-review.jpg)
---

### What percentage of non-Vine reviews were 5 stars?

![percentage-nonpaid-review](https://github.com/backwater-graphics/Amazon_Vine_Analysis/blob/main/Resources/percentage-nonpaid-review.jpg)
---

## Summary

In conclusion, the vine program might just not be worth it for the pet category. As it can be seen, there were not many helpful reviews that made part of it (total of 170), and only around half of them were 5-star rated (57%). Very similarly to the unpaid (total of 37,840), reviews which also only about half of them were 5 star rated (47%). Even though the percentages may be misleading as the volume of reviews in the vine and non-vine programs vary so much, this itself is a sign that the vine program is not very popular in this category. We might not want to pay for it as it is not incentivizing the people to write better reviews.

This allows us to conclude that customers don't feel a positivity bias for leaving good reviews in the paid program as there are so few and not so many well-rated. Nevertheless, if we were to further analyze we could calculate the mean of the star ratings on each programs' reviews to see if there's a significant incentive.
