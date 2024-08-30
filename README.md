# Bank Customer Segmentation and Attrition Analysis

This is a Data Mining project which conducted customer segmentation and attrition prediction using PCA and K-Means, achieving high predictive accuracy with random forest and gradient boosting models. It also performed Recency, Frequency, Monetary analysis on spending behavior to extract further insights.

## Table of Contents
- [Project Description](#project-description)
- [Dataset Overview](#dataset-overview)
- [Implemented Models and Results](#implemented-models-and-results)
- [Contributors](#contributors)

## Project Description
This project focuses on analyzing customer behavior within a consumer credit card portfolio to predict customer churn and better understand the factors leading to attrition. The dataset used in this study contains extensive demographic information, such as age, gender, marital status, and income category, as well as key insights into each customer’s relationship with their credit card provider. This includes details like card type, months on book, and periods of inactivity.

The primary objectives are to explore whether unsupervised methods can organically cluster customers based on their attributes and then use these clusters to predict churn labels. Additionally, the project aims to develop a predictive model to determine whether a customer is likely to churn and gain insights into customer behavior patterns that contribute to attrition.

## [Dataset Overview](https://www.kaggle.com/datasets/thedevastator/predicting-credit-card-customer-attrition-with-m/data)
This dataset contains a wealth of customer information collected from within a consumer credit card portfolio, with the aim of helping analysts predict customer attrition. It includes comprehensive demographic details such as age, gender, marital status and income category, as well as insight into each customer’s relationship with the credit card provider such as the card type, number of months on book and inactive periods. Additionally it holds key data about customers’ spending behavior drawing closer to their churn decision such as total revolving balance, credit limit, average open to buy rate and analyzable metrics like total amount of change from quarter 4 to quarter 1, average utilization ratio and Naive Bayes classifier attrition flag (Card category is combined with contacts count in 12months period alongside dependent count plus education level & months inactive). Faced with this set of useful predicted data points across multiple variables capture up-to-date information that can determine long term account stability or an impending departure therefore offering us an equipped understanding when seeking to manage a portfolio or serve individual customers

**Quick Look:**

Size: 10127 rows x 23 columns 
- No null values
- Given labels: Existing or Attrited Customer

Sufficient for Data Mining Techniques:
- Customer Attributes
- Can predict customer level from the labels
- Recency and Frequency metrics

## Analysis and Results
### Part 1: Recency, Frequency, and Monetary
Calculate the RFM score for each customer based on:

**Formula: RFM Score = 0.7*Recency + 0.3*Frequency**

*Not consider Monetary:* 
1. Churn Focus
2. Data Interpretation Challenges

**Humanization**: Under each segment designed, what's the proportion of attrited vs. existed (based on true labels)?

RFM Clustering and Strategy

### Part 2: Principal Component Analysis and Clustering 
**PCA**: 
Retain the cumulative variance explained to 90% 

**K-means**: 
Elbow Method for Optimal Cluster Determination

**Supervised Learning**: 
Predicting attrition rates for various customer segments.

- *Importance: Insightful for devising targeted retention strategies and understanding customer churn patterns to enhance retention strategies and service offerings.*
- Feature Engineering: Implemented *SMOTE* to counteract class imbalance issue, integrated K-Means clustering results (cluster labels) with selected features
- Model Performance Evaluation & Comparison

Recommendations to reduce customer churn rate

See more details [here](/Data_Mining_Project_Pre.pdf).

## Contributors
- Cailey Farrell
- Xiyi Lin
- Stella Wang
- Ye Joon Han