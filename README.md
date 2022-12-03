# Amazon_Vine_Analysis

## Overview
The purpose of this analysis was to look at a dataset of video game reviews obtained from the Amazon AWS public review data.  The dataset selected contains reviews of video games for US region with a historical time period from approximatley 2018 back to 1998. The goal was to use PySpark to perform an ETL process on the data, transform the data and connect to an AWS RDS instance, and load into pgAdmin. Then the tools of PySpark, Pandas,and SQL were used to determine if there was any bias toward favorable reviews from Vine members in the selected dataset. 

## Resources
Data Sources: [Amazon Data Review Sets](https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Digital_Video_Games_v1_00.tsv.gz) 

## Results
The analysis focused on answering the following questions with regard to the video game dataset of reviews by Vine users and there results of paid and un-paid reviews.

- How many Vine reviews and non-Vine reviews were there?

- How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

- What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

There were a total of 94 Vine reviews that were deemed helpful. Meaning the video game review had over 50 percent of its votes marked as "helpful" by other reviewers. There were a total of 40,565 reviews in all, and of those, 15,711 where 5 star reviews. 

Of the 94 Vine reviews, 48 were noted as paid reviews. This equates to 51% of the Vine reviews were 5 stars! In comparison, there were a total of 40,565 reviews in all that were deemed helpful (50 percent viewer votes).  And of those 40k, there were 15,711 5 star reviews.  This equates to a 38% of all reviews being 5 star.  

When comparing the percent of Vine 5 star reviews to the percent of all reviews, 51% vs 38%, the analysis reveals a strong bias towards paid reviews overall. See the analysis calculations and results graphic below.

<p align="center">
    <br>  <b> Analysis Results</b>  </br>
<img src="https://github.com/dfwdamon/Amazon_Vine_Analysis/blob/main/Reviews.png" width="625" height="500"/>

## Summary
The percentage of 5 star reviews for Vine customers was considerably higher than those of regular reviews.  The difference is significant as paid reviews are higher based on 5 star ratings since by being more than half, at 51%.  However, the  small set of vine reviews in all, being only 94 is a small data set when compared to all game reviews.  A larger dataset of vine reviews would likely reveal more or less bias.  Regular 5 star review data would suggest less bias both because the dataset is much larger, and there are non-paid reviews in that set.  Comparing other product review datasets of paid reviews, to the Vine review data could help show if bias is stronger toward small and larger paid and unpaid datasets.
