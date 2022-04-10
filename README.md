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
