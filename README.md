#Module 16 Challenge

# Amazon Vine Reviews Analysis

## Overview

The objective of this project is analyzing Amazon reviews written by members of the paid Amazon Vine program. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members who are then required to publish a review.
Through this project we’re practicing performing the ETL process to extract the dataset (among about 50 available), transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin as well as PySpark.
Selected data: Reviews for Musical Instruments

![ Reviews for Musical Instruments](https://github.com/TheLittlePrincess/M16_Amazon_Vine_Analysis/blob/main/Reviews%20for%20Musical%20Instruments.jpg)

## Results

•	How many Vine reviews and non-Vine reviews were there? 
Total of 904,765, 2,287 from paid users and 902,476 from unpaid ones

•	How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
To make the analysis more meaningful, and as instructed, the set was narrowed down to reviews with 20 or more votes, considerably reducing the number entries; and further down to those for which reviews marked as helpful accounted to 50% or more of the total votes. For such group 60 belong to paid users and another 14,477 to unpaid ones.

Vine Paid and unpaid subsets
![ Vine Paid and unpaid subsets](https://github.com/TheLittlePrincess/M16_Amazon_Vine_Analysis/blob/main/Vine%20Paid%20and%20unpaid%20subsets.jpg)

•	What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

It was interesting to see how the percentage of 5 stars reviews were very close between the two groups, 56.67% among paid users and 56.72% for those unpaid. Such a small difference (less than 1%) suggests that payment membership status **do not** influence the 5 star reviews in this product category. 

Note however that given how different the size of the two groups are, were reviews from paid members account for only a very small percentage of the total, further analysis to determine any positivity bias for reviews in the Vine program and/or the significance of them might be needed; for instance:
•	checking on each tier
•	Compare more than 3 stars vs less than 3 stars and/or
•	Randomize a sample from the unpaid users so that is more comparable size to the paid ones
  
Percentage of 5_Star reviews
![ Percentage of 5_Star reviews](https://github.com/TheLittlePrincess/M16_Amazon_Vine_Analysis/blob/main/Percentage%20of%205_Star%20reviews.jpg)


