![graphic](images/amz.vine.graphic.jpg)

### Overview of the Analysis: 

I was recently tasked with analyzing reviews from Amazon written by members of the paid Amazon Vine Program. The Vine program is a program in which companies pay a small fee for the members to leave mandatory reviews on products in which they have purchased. The reviews are not fabricated or false and the Amazon Vine member is in no way obligated to only leave a positive review. The program is by invitation only and there are specific criteria that one must meet in which to be invited into the program.

### Purpose of the analysis:

For my analysis I used Amazon review data pertaining to items within the outdoor category. The purpose of the analysis today was to use PySpark, an AWS database and Pg-Admin(a SQL database) to Extract, Transform, Load and Analyze the Vine Program data. Initially we will look at the number of reviews that were left by vine member and those from other members. We will also look at the quality of those reviews. Were most of the Vine program reviews 5 stars? Did being a Vine member sway the reviews in any meaningful way?

Note: Before the analysis was started the data was filtered to only include reviews with more than 20 total votes and then filtered additionally to only contain reviews where more than 50% were helpful. The starting number of reviews was: 37,544.

### Results:

#### How many Vine reviews and non-Vine reviews were there?
![graphic](images/yvinedf.png)    ![graphic](images/yvinecount.png)

![graphic](images/nvinedf.png)    ![graphic](images/nvinecount.png)
#### How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
![graphic](images/5starrating.png)
#### What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
![graphic](images/percentof5stars.both.png)
##### Vine Program 5-Star Ratings: 53.3% | Non-Vine Program 5-Star Ratings: 52.7%

### Summary: 

From my analysis of the outdoor item reviews from Amazon I can observe no obvious positivity bias . As we can see above while there were far fewer Vine program member reviews there were still almost identical 5-star rating percentages, 53.3% and 52.7% respectively.

An additional analysis that we could do would be to look at the spread of the other ratings for Vine program members. Do they skew in to the 3-5 range or are they "evenly" distributed? I would also want to look at additional datasets to compare the ratings.

