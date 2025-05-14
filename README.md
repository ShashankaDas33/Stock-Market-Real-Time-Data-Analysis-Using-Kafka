# 📈 Stock Market Real-Time Data Analysis Using Kafka (AWS-Based)

This project demonstrates a real-time stock market data processing pipeline using **Apache Kafka** hosted on **AWS EC2**, integrated with **Amazon S3**, **AWS Glue**, and **Amazon Athena** for data storage, cataloging, and querying.

---

## 🧠 Architecture Overview

![Architecture](./Architecture.jpg)

### Components:

- **Stock Market App Simulation**:
  - Simulates stock data using a CSV dataset.
  - Written in Python and uses `boto3` SDK.
  - Acts as a Kafka **Producer**.

- **Apache Kafka (on Amazon EC2)**:
  - Acts as the backbone for real-time streaming.
  - Handles message queuing between producer and consumer.

- **Kafka Consumer**:
  - Consumes stock market data.
  - Stores it in **Amazon S3** in real-time.

- **AWS Glue**:
  - **Crawler** scans data in S3 and updates the **Glue Data Catalog**.

- **Amazon Athena**:
  - Used to perform SQL queries on the stock data for real-time analytics.

---

## 🔧 Technologies Used

- Python (with `boto3`, `kafka-python`)
- Apache Kafka (deployed on EC2)
- Amazon S3
- AWS Glue & Glue Crawlers
- Amazon Athena
- CSV Dataset

---



