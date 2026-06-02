# AI-Based-Customer-Behavior-Campaign-Prediction-System
# Overview

This project analyzes customer purchasing behavior and evaluates the effectiveness of retail marketing campaigns using transactional, demographic, coupon, and promotional data from the Dunnhumby "The Complete Journey" dataset.

The objective is to determine whether promotional campaigns drive long-term customer loyalty or simply create short-term increases in sales. Using machine learning, uplift modeling, recommendation systems, and customer engagement analysis, the project provides data-driven insights to improve marketing ROI and customer targeting strategies.

# Business Problem

Retailers invest significant resources in promotional campaigns, discounts, and coupons. However, many organizations struggle to determine:

Which customers are genuinely influenced by promotions
Whether campaigns increase long-term loyalty
How discounts affect purchasing behavior
Which customer segments generate the highest return on investment

This project addresses these challenges through predictive analytics and customer behavior modeling.

# Dataset

Source: Dunnhumby - The Complete Journey Dataset

The project integrates multiple datasets including:

Transaction Data
Product Information
Customer Demographics
Campaign Data
Coupon Data
Coupon Redemption Data
In-Store Promotion Data
Dataset Characteristics
2.5+ Million Transaction Records
2,500 Customer Households
92,000+ Products
30 Marketing Campaigns
2 Years of Retail Purchase History
Project Objectives
Store Performance Analysis

Evaluate store performance using:

Average Spend per Household
Trip Frequency
Category Breadth
Customer Loyalty Analysis

Identify drivers of long-term customer engagement through:

Purchase Frequency
Weeks Active
Department-Level Activity
Campaign Impact Analysis

Measure changes in:

Customer Spending
Shopping Trips
Coupon Redemptions
Customer Segmentation

Analyze customer behavior across:

Income Groups
Age Categories
Household Sizes
Brand Preferences

Discount Dependency Analysis

Determine how heavily customers rely on discounts and promotions.

Data Preparation

Key preprocessing steps included:

Missing Value Treatment
Data Standardization
Duplicate Removal
Outlier Detection & Treatment
Feature Engineering
One-Hot Encoding
Feature Scaling
Analytical Base Table (ABT) Creation

Dataset omitted due to size limitations.
Original dataset available from the source:
https://www.dunnhumby.com/sourcefiles/

# Machine Learning Models
# 1. Uplift Modeling

Purpose:
Identify customers whose behavior is directly influenced by marketing campaigns.

Technique:

Random Forest Classifiers
Treatment vs Control Analysis
Qini Curve Evaluation
AUUC Analysis

# 2. Product Recommendation System

Purpose:
Recommend products based on purchasing patterns.

Technique:

Cosine Similarity
Product-to-Store Revenue Matrix

# 3. Coupon Recommendation Model

Purpose:
Personalize discount allocation for customers.

Technique:

XGBoost Classifier
Behavioral Feature Engineering

# 4. Campaign Effectiveness Model

Purpose:
Measure customer spending changes before and after campaigns.

Technique:

Customer-Level Spending Analysis
Predictive Classification

# 5. Customer Engagement Predictor

Purpose:
Predict long-term customer engagement.

Technique:

Random Forest Classifier
GridSearchCV Hyperparameter Tuning

# Results
# Uplift Model
Validation AUUC: 6.56
Test AUUC: 6.09
Validation Qini: 33.47
Test Qini: 22.69

Key Finding:
Only a small segment of customers were truly influenced by campaigns.

# Coupon Recommendation Model
Test Accuracy: 62.8%
Test AUC: 0.686
Test F1 Score: 0.571

Key Finding:
Personalized discounts outperform blanket promotions.

# Campaign Effectiveness
Average Spending Increase: +2.6%
55.1% Customers Increased Spending
Test AUC: 0.664

Key Finding:
Campaign impact varies significantly across customer groups.

# Customer Engagement Predictor
Test Accuracy: 72%
Test Recall: 90%
Test AUC: 0.86

Key Finding:
Purchase frequency and recency are stronger indicators of loyalty than discount usage.

# Key Business Insights
Approximately 75% of targeted customers are "Sure Buyers" who would purchase regardless of promotions.
Deep discounts do not necessarily create long-term loyalty.
Customer engagement is driven primarily by purchase frequency and shopping recency.
Personalized marketing strategies significantly improve promotional efficiency.
Data-driven coupon allocation can reduce unnecessary promotional spending.
Technologies Used
Programming Language
Python
Data Analysis
Pandas
NumPy
Data Visualization
Matplotlib
Seaborn
Machine Learning
Scikit-Learn
XGBoost
Modeling Techniques
Random Forest
Uplift Modeling
Recommendation Systems
Classification Models

# Development Environment
Google Colab

Jupyter Notebook
