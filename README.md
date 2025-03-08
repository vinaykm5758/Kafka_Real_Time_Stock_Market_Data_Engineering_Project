# Kafka_Real_Time_Stock_Market_Data_Engineering_Project
This Repo contains details about Kafka Real Time Stock Market Data Engineering Project, Thanks

Introduction

In this project, you will execute an End-To-End Data Engineering Project on Real-Time Stock Market Data using Kafka.
We are going to use different technologies such as Python, Amazon Web Services (AWS), Apache Kafka, Glue, Athena, and SQL
Extension to the technologies made includes:
1. Connecting PowerBI to AWS S3 JSON File and building a sample PowerBI Report
2. Connecting PowerBI to AWS Athena Database and building a sample PowerBI Report

![image](https://github.com/user-attachments/assets/c7927d75-fa00-4328-af21-94cdd66a756c)

**Technology Used:**

1. Programming Languages: Python and R Language
2. Cloud Provider: AWS - S3, Athena, Glue Catalog, Glue Crawler, Ec2
3. Reporting Tool: PowerBI
4. ODBC Driver: Simba ODBC Driver to connect PowerBI to AWS Athena
5. R Packages: AWS S3 R Package to connect to AWS S3 bucket

**Dataset URL:** https://github.com/vinaykm5758/Kafka_Real_Time_Stock_Market_Data_Engineering_Project/blob/main/indexProcessed.csv

Kafka Producer Code: https://github.com/vinaykm5758/Kafka_Real_Time_Stock_Market_Data_Engineering_Project/blob/main/Kafka_Producer.ipynb
Kafka Consumer Code: https://github.com/vinaykm5758/Kafka_Real_Time_Stock_Market_Data_Engineering_Project/blob/main/KafkaConsumer.ipynb
Connecting to Kafka components in AWS EC2 Instance: https://github.com/vinaykm5758/Kafka_Real_Time_Stock_Market_Data_Engineering_Project/blob/main/Kafka_1.PNG

AWS S3 Data: https://github.com/vinaykm5758/Kafka_Real_Time_Stock_Market_Data_Engineering_Project/blob/main/AWS_S3_Data.PNG


**PowerBI Reports:**
1. Connecting PowerBI with AWS S3 bucket sample JSON file: **Page-1**: https://github.com/vinaykm5758/Kafka_Real_Time_Stock_Market_Data_Engineering_Project/blob/main/Realtime_AWS_Athena_PowerBI_Report.pbix
2. Connecting PowerBI with AWS Athena Table "stock_market_kafka.kafka_stock_market_demo_viinay": **Page-2**: https://github.com/vinaykm5758/Kafka_Real_Time_Stock_Market_Data_Engineering_Project/blob/main/Realtime_AWS_Athena_PowerBI_Report.pbix

**Data Validations:**
1. Validated the counts for the Index column from AWS Athena Vs PowerBI Report in Real time: **Counts Matched**

   ![image](https://github.com/user-attachments/assets/ef2b7e00-5e88-4380-8fe5-100bcca82893)


   ![image](https://github.com/user-attachments/assets/a641031f-e1e0-4dad-a8ac-f992ee93d1cb)

   

**R Script used in PowerBI:**

Sys.setenv(

  "AWS_ACCESS_KEY_ID" = 'XXX',
  "AWS_SECRET_ACCESS_KEY" = 'XX',
  "AWS_DEFAULT_REGION" = "us-east-1"
)

test_data <- aws.s3::s3read_using(FUN = read.csv,
                                  object = 'stock_market_95.json',
                                  bucket = 's3://kafka-stock-market-demo-viinay/')
								  
								  

								  




