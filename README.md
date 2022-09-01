# Predict Customer Personality to Boost Marketing Campaign by Using Machine Learning
## Background
A company can develop rapidly when it knows the behavior of its customer personality, so that it can provide better services and benefits to customers who have the potential to become loyal customers.
Company need to know it's customer behavior to boost marketing campaign.
### Goal
Improve marketing campaign performance and target the right customers to be able to do transaction(s) on the company's platform.
### Objective 
Create a cluster prediction model using unsupervised learning so that it makes easier for companies to make decisions.
## Data
Dataset contains customer behavior features who made transactions and interactions on our platform.
## Tools
On this project I've used python as programming language; jupyterlab as notebook; pandas, numpy, sklearn and dython to preprocessing and machine learning section; combination of matplotlib and seaborn library to generated data visualization.
## Contents
### **Exploratory Data Analysis**
### **Data Cleaning and Preprocessing**
On this section, there are few processes such as handling missing and duplicated value, feature selection using RFMLC (Recency, Frequency, Monetary, Loyalty and C) methods, handling outliers using IQR (Q1=1%; Q3=99%), feature transformation to selected features using minmaxscaler, and splitting data on 70:30 proportion.
### **Data Modeling**
Using K-Means Clustering with cross-validation elbow method to inertia and silhoutte score
### **Customer Persoality Analysis for Marketing Retargeting**
Based on my model, there are 4 customer clusters:
1. High-Valued Customer:
Customers on this group have `high average recency (73 days)` and `high average of total purchases (21 items)` it means they are not frequent shoppers but they spend a lot on our platform `(around IDR 1M/year)`.
2. Low-Valued Customer:
Customers on this group `have highest average recency (74 days)` and `low average of total purchases (8 items)` it means they are not frequent shoppers and they spend a little on our platform `(around IDR 92K/year)`.
3. High-Valued Frequent Customer:
Customers on this group `have low average recency (23 days)` and `high average of total purchases (21 items)` it means they are frequent shoppers and they spend a lot on our platform `(around IDR 989K/year)`.
4. Low-Valued Frequent Customer:
Customers on this group `have high average recency (24 days)` and `lowest average of total purchases (7 items)` it means they are frequent shoppers but they spend a little on our platform `(around IDR 75K/year)`.
### **Recommedation**
#### Actionable Isights
1. Create membership tier program to keep customer retention also membership tier things will attract customers to shopping more on our platform. Let's say we have 4 membership tier (Platinum, Gold, Silver, Bronze) each membership tier has different privilages as customers. The highest membership tier they have, the greatest privilages they will get. On this case, we can give membership tier based on customer clusters (Platinum: High-Valued Customer, Gold: High-Valued Frequent Customer, Silver: Low-Valued Frequent Customer, Bronze: Low-Valued Customer)
2. Prioritize to focus on High-Valued Customers group to avoid the risk of churn. Keep monitoring theirs purchases trend and keep their retention such as improve our service, after sales treatment, quality of our products and apps. Beside that, we can give them the highest membership tier (Platinum Tier) at this case we can give them more discounts, promotions and free-shipping cost than any membership tier to make them shopping on our platform more frequent
3. Give High-Valued Frequent Customer group more promotions or free-shipping cost coupon through our membership tier program to make them shopping on our platform more frequent.
4. Since on Low-Valued Frequent Customer and Low-Valued Customer have lowest total spend on our platform, we should create more personalization ads, promotions or campaign for low cost products to attract this groups to shopping on our platform. Potentially this strategy will improve they recency (to low) and total of purchases (to high) on low cost products.
#### Potential Impact (Quantitative)
If we keep prioritize on Customer Groups/Clusters and they do not turn to churn, we still have potential GMV around IDR 1.3B/year (High-Valued Customer=IDR 670M/year; Low-Valued Customer=IDR 46M/year; Low-Valued Frequent Customer=IDR 604M/year; Low-Valued Customer=IDR 47M/year).
