# Udacity Capstone Project Starbucks

## Project Overview and Motivation
This analysis was conducted as part of the Udacity Data Scientist Nanodegree program, serving as a capstone project.
The goal of sending advertisements and offers to customers is to increase their purchases. However, it would be naive to send all offers to all customers simultaneously. This project aims to utilize transactional and demographic data to identify offers tailored to different customer segments.
In the realm of data-driven marketing strategies, understanding customer behavior remains a cornerstone for personalized outreach. This blog post explores the relationship between demographic characteristics and offer fulfillment within the Starbucks Rewards program. The analysis focuses on key variables such as age, income, gender, and spending at Starbucks, examining their influence on the likelihood of customers accepting offers.

## Description of Input Data
Starbucks has provided a dataset simulating customer behavior while using the Starbucks Rewards Mobile App. The app allows customers to receive promotions and offers, as well as make payments in-store. Starbucks sends various advertisements and offers to customers every few days, which can include:

The Starbucks dataset is contained in three files in the 'data' folder:
-	portfolio.json + portfolio.csv : Contains offer IDs and metadata for each offer (duration, type, etc.).
-	profile.json + profile.csv: Contains demographic data for each customer.
- transcript.csv: Records transactions, received, viewed, and completed offers. (transcript.json was too big to upload).

## Approach
Data Preprocessing: Included handling missing values, encoding categorical variables, and feature engineering.
Exploratory Data Analysis (EDA): Analyzed patterns, distributions, and relationships within the data to gain insights.
Model Development: Built up and optimized machine learning models, considering feature importance and prediction accuracy.
Evaluation: Utilized metrics such as accuracy and F1 score to assess the model's performance.

## Key Findings
Model Accuracy: The Gradient Boosting Classifier achieved an impressive accuracy score of 91%, showcasing its proficiency in predicting offer completion within the Starbucks rewards program.
Feature Importance: Time, reward, and income emerged as the most critical factors influencing offer completion, guiding strategic decision-making.
Model Robustness: With an F1 score of 0.91 for class 0 and 0.59 for class 1, the model displays a balanced approach in accurately identifying completed offers.

## Conclusion
The project aimed to bridge the gap between demographic characteristics and offer completion rates. By leveraging machine learning techniques, it sought to provide actionable insights for targeted marketing strategies and personalized offer recommendations, benefiting the Starbucks rewards program and enhancing customer engagement.
Accuracy Score:
The Decision Tree Classifier achieved an average accuracy of 86% after extensive fine-tuning and optimization. This demonstrates the model’s fundamental ability to correctly predict offer completions in the Starbucks rewards program.
F1 Score and Model Robustness:
Furthermore, the model’s evaluation metrics show robust performance. With an F1 score of 0.94 for class 0 and only 0.30 for class 1, the model achieves a limited balance between precision and recall. This is particularly restricted when predicting features that have a value of 1 compared to those that have a value of 0.
Reflection of Accuracy:
While accuracy is a fundamental indicator of model performance, the supplementary evaluation based on precision, recall, and F1 score provides a more nuanced understanding of the model’s predictive power.

The models clearly exhibit the issue of class imbalance (unequal class distribution). In the dataset, there are many more examples of the negative class (class 0) than of the positive class (>0). This was further exacerbated by the transformation of columns with binary values. This can lead to the model tending to favor the negative class, resulting in poor performance in detecting the positive class.

## Medium Article
https://medium.com/@marc.hammer/udacity-capstone-project-starbucks-575edace06a2

