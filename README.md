#Amazon_Vine_Analytics
Big Data: Week 16
# Amazon_Vine_Analytics
Working with Big Data through Spark in Google Collab & AWS 
## Overview of Amazon_Vine_Analytics:
Since your huge success with your first project on SellBy, you have been given another project. This time you are working with a bigger client Amazon. They want you and Jennifer to work on Amazon’s Vine program which sets up how publishers and manufactures view the reviews of their products. For this project we will choose from 1 of 50 datasets so we can extract, transform and load the data, then using the AWS systems we will move the tables into PgAdmin. The using one of three systems PySpark, Pandas or SQL you will determine if there is any bias towards favorable reviews in the dataset. For this project we choose to work on the amazon reviews for pet products and analyzed the dataset using PySpark. 
#### The below pseudocode provided us an outline for the analysis ####
Deliverable 1: Perform ETL on Amazon Product Reviews
Deliverable 2: Determine Bias of Vine Reviews
Deliverable 3: A Written Report on the Analysis (README.md)

1.	### Perform ETL on Amazon Product Reviews:

•	#### Customers_df ####


![alttext](https://github.com/mbehr11/Amazon_Vine_Analytics/blob/main/Resources/customers_df.PNG) 

•	#### Products_df ####


![alttext](https://github.com/mbehr11/Amazon_Vine_Analytics/blob/main/Resources/products_df.PNG)

•	#### Review_id_df ####

![alttext](https://github.com/mbehr11/Amazon_Vine_Analytics/blob/main/Resources/review_id_df.PNG)

•	#### Vine_df ####

![alttext]( https://github.com/mbehr11/Amazon_Vine_Analytics/blob/main/Resources/vine_df.PNG)

•	#### Load the DataFrames into PgAdmin 

•	Customers_table:

![alttext](https://github.com/mbehr11/Amazon_Vine_Analytics/blob/main/Resources/customers_table_SQL.PNG)
•	Products_table:
![alttext](https://github.com/mbehr11/Amazon_Vine_Analytics/blob/main/Resources/products_table_SQL.PNG)
•	Review_id_table:
![alttext](https://github.com/mbehr11/Amazon_Vine_Analytics/blob/main/Resources/review_id_table_SQL.PNG)
•	Vine_table:
![alttext](https://github.com/mbehr11/Amazon_Vine_Analytics/blob/main/Resources/vine_table_SQL.PNG)

2.	### Deliverable 2: Determine Bias of Vine Reviews:

•	Vine_table:
![alttext](https://github.com/mbehr11/Amazon_Vine_Analytics/blob/main/Resources/pet_products_df.PNG)
•	Filtered_df for 20 or more votes and where the prefect is greater than 50%:
![alttext](https://github.com/mbehr11/Amazon_Vine_Analytics/blob/main/Resources/filtered_df.PNG)
•	The data is filtered to create a DataFrame or table where there is a Vine review:
![alttext](https://github.com/mbehr11/Amazon_Vine_Analytics/blob/main/Resources/paid_5_star_df.PNG)


•	The data is filtered to create a DataFrame or table where there isn’t a Vine review:
![alttext](https://github.com/mbehr11/Amazon_Vine_Analytics/blob/main/Resources/unpaid_5_star_df.PNG)
•	The total number of reviews, the number of 5-star reviews, and the percentage 5-star reviews are calculated for all Vine and non-Vine reviews:

![alttext](https://github.com/mbehr11/Amazon_Vine_Analytics/blob/main/Resources/paid_vs_unpaid_df.PNG)
3.	### Summary of Amazon_Vine_Analytics: 
For this set of data there is no positivity bias for the Vine program. As the data suggests the negative reviews were more helpful in people deciding to purchase the product than the positive reviews. As we can see we have 38% for paid and 54% for unpaid. For further analysis, I would do a prediction model using the standard deviation for future products. I would also take the filtered dataframe and preform a summary specially looking at the standard deviation to determine what key words were triggering people to buy products or not. I would also see how often non vine users were purchasing items vs vine users. 

## Contributing 
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)
