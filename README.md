# Amazon_Vine_Analysis

## Tools
* PySpark
* Jupyter Notebook
* Python
* AWS
* SQL
* Google Colab


## Overview of the Analysis
The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. For this project the goal is to analyze reviews written by members of the paid Amazon Vine program. Companies pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review. There are numerous product categories that are a part of the Vine program. This analysis focused on 'Digital Video Downloads' and the reviews provided for this category of products. The goal of the analysis is to determine if there is any bias toward favorable reviews from Vine members. 

To complete the analysis the ETL process was performed on the Amazon dataset using Amazon Web Servies RDS and Pyspark. Next the data was loaded into a SQL database and the review data was analyzed using Pandas. 

## Results

- The total number of Vine and non-Vine reviews was determined as part of the analysis. In this dataset there were a total of 5,879 Vine reviews and a total of 4,638 non-Vine reviews. 

    ![Vine_Reviews Screenshot ](https://user-images.githubusercontent.com/96552268/166148338-72a4dc86-0720-45d4-8915-b34db8a36a40.png)
    ![NonVine_Reviews Screenshot ](https://user-images.githubusercontent.com/96552268/166148343-70deaf53-fd68-4b7f-87dd-e8e2c3942e82.png)

- Next we determined the total number of 5-star reviews for both Vine and non-Vine members. There were a total of 2,582 5-star reviews from Vine members and 1,791 5-star reviews from non-Vine members. 

  ![5 Star Review Count Screenshot](https://user-images.githubusercontent.com/96552268/166148438-cf9a56a8-114c-42a4-833b-77d650f67e30.png)

- Lastly we used the analysis data to determine the percentage of 5-star reviews for each type of customer. 44% of Vine member reviews were 5-star compared with non-Vine members who had 39% of their reviews as 5-star.


  ![5 Star Review Percentage Screenshot](https://user-images.githubusercontent.com/96552268/166148599-527e2c31-631c-4df5-8b22-9bddee33334c.png)

## Summary

Based on the analysis of the dataset there is a tendency for Vine members to submit a higher percentage of 5-star reviews than non-Vine members. The overall average of reviews that are 5-star for the entire dataset is 42% showing that Vine members submit 5-star ratings at a rate that is above the average and non-Vine members submit 5-star reviews at a rate below the average.  

###### Additional Analysis

To further determine if there is a bias towards positive reviews for Vine members the analysis could also be performed on the number of 4-star ratings submitted by Vine and non-Vine members to see if the trend continues. Additionally statistical analysis could performed on the dataset to determine if the difference in the percentage of positive reviews submitted by Vine members is statistically significant. 
