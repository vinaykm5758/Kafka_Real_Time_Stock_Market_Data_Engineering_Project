# Kafka_Real_Time_Stock_Market_Data_Engineering_Project
This Repo contains details about Kafka Real Time Stock Market Data Engineering Project, Thanks

Introduction

In this project, you will execute an End-To-End Data Engineering Project on Real-Time Stock Market Data using Kafka.
We are going to use different technologies such as Python, Amazon Web Services (AWS), Apache Kafka, Glue, Athena, and SQL
Extension to the technologies made includes:
1. Connecting PowerBI to AWS S3 JSON File and building a sample PowerBI Report
2. Connecting PowerBI to AWS Athena Database and building a sample PowerBI Report

![image](https://github.com/user-attachments/assets/c7927d75-fa00-4328-af21-94cdd66a756c)

Technology Used:

1. Programming Languages: Python and R Language
2. Cloud Provider: AWS - S3, Athena, Glue Catalog, Glue Crawler, Ec2
3. Reporting Tool: PowerBI
4. ODBC Driver: Simba ODBC Driver to connect PowerBI to AWS Athena
5. R Packages: AWS S3 R Package to connect to AWS S3 bucket

Dataset URL:

PowerBI Reports:

R Script:

Sys.setenv(

  "AWS_ACCESS_KEY_ID" = 'XXX',
  "AWS_SECRET_ACCESS_KEY" = 'XX',
  "AWS_DEFAULT_REGION" = "us-east-1"
)

test_data <- aws.s3::s3read_using(FUN = read.csv,
                                  object = 'stock_market_95.json',
                                  bucket = 's3://kafka-stock-market-demo-viinay/')
								  
								  

								  




