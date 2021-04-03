# Amazon_Vine_Analysis

## Overview

I investigated whether there was any bias towards reviews written as part of the Vine Program from Amazon, INC.

To do this, I used Google Colaboratory as well as Pyspark to perform the Extract, Transform and Load process. I also loaded the data into a relational database in PGAdmin. Lastly, I created filtered dataframes from the original dataset after processing to discover any bias with vine reviews.

## Results

The following output from the notebook shows the results from the filtering:

![Summary_Vine](https://github.com/Kyle2Miles93/Amazon_Vine_Analysis/blob/main/Resources/Summary_Vine.png)


* There were **26** total reviews for paid vine programs.
* There were **29,264** total reviews for unpaid ones.

* There were **5** five-star rated reviews for the paid vine programs
* There were **15,784** five star reviews for those that were unpaid

* I calculated the precentage of each type of vine and got these results:

    - 34.62% were five star ratings in the **paid** dataframe...
    - 53.94% were five stars in the **unpaid** dataframe.

## Summary

* There seems to be a strong positivity bias in favor of reviews which are unpaid. 
  - This could be because there are a lot more of them as compared to the ones that are from paid vines.

* Another analysis using this dataset to support the above statement is perhaps a statistical one, like a sample T-Test. 
* This would show exactly how skewed and biased the results were based on the p-value generated from T-Tests on both paid / unpaid Dataframes.
