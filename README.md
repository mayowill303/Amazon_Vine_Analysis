# Amazon_Vine_Analysis
- This module helps define big data and describe the challenges associated with it.
- Define Hadoop and name the main elements of its ecosystem.
- Explain how MapReduce processes data.
- Define Spark and explain how it processes data.
- Describe how NLP collects and analyzes text data.
- Explain how to use AWS Simple Storage Service (S3) and relational databases for basic cloud storage.
- Complete an analysis of an Amazon customer review.

## Summary
In this project, we have access to approximately 50 datasets. Each one contains reviews of a specific product, from clothing apparel to wireless products. I chose home improvement revidws and used PySpark to perform the ETL process to extract the reviews, transform the data about the reviews, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, I used PySpark, Pandas, or SQL to determine if there is any bias toward favorable reviews from Vine members in the dataset. Then, I wrote a summary of the analysis for Jennifer to submit to the SellBy stakeholders.

### Results

#### Deliverable 1 Requirements
An Amazon Review dataset is extracted as a DataFrame (10 pt)

![Amazon Review dataset](https://user-images.githubusercontent.com/96395120/162639541-eac9b529-33c1-4db8-ae49-5f94a7ea8340.png)

The extracted dataset is transformed into four DataFrames with the correct columns (20 pt)

![extracted dataset-1](https://user-images.githubusercontent.com/96395120/162639615-ec48f003-5dd0-44f4-a84c-6d2ef056b79a.png)
![extracted_dataset-2](https://user-images.githubusercontent.com/96395120/162639680-c89ddcec-42b7-4b76-9e63-c1eb94f2459d.png)
![extracted_dataset-3](https://user-images.githubusercontent.com/96395120/162639734-e1c490e4-5d7e-44ae-9756-cb0075efea4b.png)
![extracted_dataset-4](https://user-images.githubusercontent.com/96395120/162639823-ad03b9e8-bf21-46bc-89c2-768843a3d724.png)

All four DataFrames are loaded into their respective tables in pgAdmin (10 pt)

![Respective Tables](https://user-images.githubusercontent.com/96395120/162652359-feff6824-cce6-41a8-8eb4-6acedea79e42.png)

#### Deliverable 2: Determine Bias of Vine Reviews
Using knowledge of PySpark, Pandas, or SQL, we determine if there is any bias towards reviews that were written as part of the Vine program. For this analysis, we determine if having a paid Vine review makes a difference in the percentage of 5-star reviews.

DataFrame or table for the vine_table data using one of three methods above (5 pt)

![vine_table_data](https://user-images.githubusercontent.com/96395120/162660831-169d9eef-dcdd-47f6-8780-f759ed97e096.png)

The data is filtered to create a DataFrame or table where there are 20 or more total votes (5 pt)

![20_or_more_votes](https://user-images.githubusercontent.com/96395120/162660941-f6d55b1d-f647-4ef1-a5cc-f2fdee39b857.png)

The data is filtered to create a DataFrame or table where the percentage of helpful_votes is equal to or greater than 50% (5 pt)

![helpful_votes](https://user-images.githubusercontent.com/96395120/162661032-76fac637-7bf0-46d0-b6aa-9a786da5fe4e.png)

The data is filtered to create a DataFrame or table where there is a Vine review (5 pt)

![vine_reviews](https://user-images.githubusercontent.com/96395120/162661088-77e9277e-66cc-4652-8980-c42ab39213da.png)

The data is filtered to create a DataFrame or table where there isn’t a Vine review (5 pt)

![no_vine_reviews](https://user-images.githubusercontent.com/96395120/162661149-93305416-6f7d-484e-8376-98830f8962cb.png)

The total number of reviews, the number of 5-star reviews, and the percentage 5-star reviews are calculated for all Vine and non-Vine reviews (15 pt)

![reviews-breakdown](https://user-images.githubusercontent.com/96395120/162661288-2c584a40-f673-41a5-8790-dd8146fb8414.png)
