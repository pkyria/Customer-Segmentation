# Customer Segmentation & Predictive Analytics Project

This project focuses on customer segmentation and predictive analytics using a combination of **Power BI reports**, **Python-based data science models**, and **machine learning techniques**. It aims to help businesses better understand their customer base, reduce churn, and improve sales forecasting.

---

## Project Components

### 1. Dataset Overview

The dataset consists of **2,000 customer transactions** from an e-commerce website, collected **daily after the “Add to Cart”** step of the customer journey. The data spans from **2019 to 2023** and includes a wide range of variables, each designed to provide detailed insights into customer behavior, order flow, and transactional outcomes.

Each transaction is uniquely identified to maintain data integrity and facilitate robust analytics.

#### Features

| Variable               | Type             | Description                                                                 |
|------------------------|------------------|-----------------------------------------------------------------------------|
| `SessionStart`         | Date              | Timestamp when the customer session started                                |
| `CustomerID`           | Integer / Unique | Unique identifier for each customer                                        |
| `FullName`             | String            | Full name of the customer                                                  |
| `Gender`               | String            | Gender of the customer                                                     |
| `Age`                  | Numerical         | Age of the customer                                                        |
| `CreditScore`          | Numerical         | Customer's credit score                                                    |
| `MonthlyIncome`        | Numerical         | Estimated monthly income                                                   |
| `Country`              | Categorical       | Country of the customer                                                    |
| `State`                | Categorical       | State or region within the country                                         |
| `City`                 | Categorical       | City of the customer                                                       |
| `Category`             | Categorical       | Product category                                                           |
| `Product`              | String            | Specific product name                                                      |
| `Cost`                 | Numerical         | Cost price of the product                                                  |
| `Price`                | Numerical         | Selling price of the product                                               |
| `Quantity`             | Numerical         | Number of units added to the cart                                          |
| `CampaignSchema`       | Categorical       | Marketing campaign classification                                          |
| `CartAdditionTime`     | Date              | Timestamp when the product was added to the cart                           |
| `OrderConfirmation`    | Boolean           | Whether the customer confirmed the order                                   |
| `OrderConfirmationTime`| Date              | Timestamp of order confirmation                                            |
| `PaymentMethod`        | Categorical       | Payment method used by the customer                                        |
| `SessionEnd`           | Date              | Timestamp when the customer session ended                                  |
| `OrderReturn`          | Boolean           | Whether the order was returned                                             |
| `ReturnReason`         | Categorical       | Reason for return (if applicable)                                          |

---
This analysis extends to 5 main dimensions that will help us extract useful information for the dataset:

- Demographic analysis
- Geographical analysis
- Product-related analysis
- Transactional analysis
- Post-purchase analysis

The methodologies we are going to use to analyze dataset is descriptive and predictive. We firstly focus on understanding better the data and try to extract insights over data anomalies or correlations among values, analyze various events and behaviors and on the final stage, this analysis,will include **Reference-Frequency-Monetary Value (RFM)**, clustering techniques, and machine learning models for purchase probability prediction and revenue forecasting, based on the dataset provided

--- 

### 2. Power BI Reports
Interactive dashboards providing insights into:
- Customer demographics and behavior
- Sales performance trends
- Segment-specific KPIs

> Located in: `powerbi_reports/`

---

### 3. Python Notebooks
Jupyter notebooks for data preprocessing, exploration, and modeling.

#### Segmentation via Clustering
- Techniques: K-Means, Principal Component Analysis (to reduce complexity)
- Purpose: Identify distinct customer groups for targeted marketing

#### Churn Prediction
- Model: Logistic Regression
- Goal: Predict the likelihood of a customer leaving (churn)
- Metrics: Accuracy, Precision, Recall

#### Sales Forecasting
- Model: XGBoost Regressor
- Task: Predict future sales volumes using time series and customer behavior data

> Located in: `python_notebooks/`

---
