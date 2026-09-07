# Customer Shopping Behaviour Analysis

## 📌 Project Overview
This project analyzes customer shopping behaviour to understand sales performance, customer characteristics, purchasing patterns, payment preferences, subscription status, and product/category performance.
The analysis follows an end-to-end data analytics workflow:

**Python Data Cleaning & EDA → SQL Business Analysis → Power BI Dashboard → Machine Learning Prediction**

## 🎯 Problem Statement
A retail business wants to better understand its customers' shopping behaviour in order to improve sales performance, customer engagement, retention, and marketing strategies.
The business has collected customer transaction data containing information about customer demographics, products purchased, product categories, purchase amounts, previous purchases, purchase frequency, subscription status, discounts, payment methods, shipping types, locations, seasons, and review ratings.
However, raw customer transaction data does not clearly reveal which products and categories perform best, which customer groups contribute the most revenue, how purchasing behaviour varies across demographics and locations, or which factors are associated with repeat purchases and customer engagement.

The management team is particularly interested in understanding:
Which products and categories generate the highest sales and revenue?
How does purchasing behaviour vary across age groups, genders, purchase frequencies, and locations?
How do subscriptions, discounts, previous purchases, and payment methods influence customer spending behaviour?
How can these insights be used to improve customer targeting, product strategy, and retention?


## 🎯 Business Objectives
The project aims to answer important business questions such as:

- What are the total sales and average transaction value?
- Which products generate the highest sales?
- Which product categories contribute the most revenue?
- Which customer groups contribute the most to sales?
- What is the distribution of subscribed and non-subscribed customers?
- Which purchase frequencies generate the most revenue?
- Which payment methods are most commonly used?
- Which locations generate higher sales?
- How does sales performance vary across gender and age groups?
- How can customer purchasing behaviour be used to support business decisions?

---

## 📊 Dataset
**Source:** Kaggle

**Records:** 3,900 customer records

### Key Fields

- Customer ID
- Age
- Gender
- Item Purchased
- Category
- Purchase Amount
- Previous Purchases
- Frequency of Purchases
- Payment Method
- Location
- Subscription Status
- Discount Applied
- Promo Code
- Season
- Review Rating
- Shipping Type
- Size
- Color

# 🔄 Workflow of Analytics

## 1. 🧹 Data Cleaning & Preparation
Python was used to inspect and prepare the raw dataset before performing further analysis.

### Activities Performed
1. Loaded and inspected the dataset.
2. Checked dataset structure and data types.
3. Identified missing values.
4. Checked duplicate records.
5. Examined categorical and numerical columns.
6. Handled data quality issues.
7. Converted columns into appropriate data types.
8. Created additional analytical fields.
9. Prepared the cleaned dataset for further analysis.

### Additional Fields Created
- `age_group`
- `purchase_frequency_days`

These fields were later used for customer segmentation and purchasing behaviour analysis.


## 2. 📈 Exploratory Data Analysis (EDA)
Exploratory Data Analysis was performed using Python to understand the structure and behaviour of the data before building the final dashboard.

### EDA Included
- Univariate analysis
- Categorical variable analysis
- Numerical variable analysis
- Distribution analysis
- Customer demographic analysis
- Purchase behaviour analysis
- Sales analysis
- Relationship analysis between important variables

### Python Libraries Used
- Pandas
- NumPy
- Matplotlib
- Seaborn

EDA helped identify patterns and relationships that were later converted into business questions and dashboard visuals.


## 3. 🗄️ SQL Business Analysis
SQL was used to perform business-focused analysis on the cleaned customer dataset and answer key business questions.

### Analysis Covered
- Revenue comparison across customer genders
- Customers who used discounts but spent above average
- Top products based on average review ratings
- Comparison of spending across shipping types
- Spending behaviour of subscribed vs. non-subscribed customers
- Products with the highest discount usage
- Customer segmentation based on previous purchases
- Top products within each category
- Relationship between repeat purchases and subscription status
- Revenue contribution across different age groups

The SQL analysis helped convert raw customer data into specific business questions, measurable metrics, and actionable insights.


## 4. 📊 Power BI Dashboard & Visualization
The final analysis was transformed into an interactive Microsoft Power BI dashboard to present the major findings in a clear and business-friendly format.

### KPI Metrics
- Total Customers
- Total Sales
- Average Transaction
- Average Rating

### Dashboard Visualizations
- Top 10 Products by Sales
- Sales by Category
- Customer Subscription Status
- Sales by Purchase Frequency
- Sales by Gender
- Sales by Age Group
- Sales by Location
- Payment Method Distribution

### Interactive Filters
- Gender
- Category
- Age Group
- Season
- Discount Applied

## 5. 🤖 Predictive Analysis – Subscription Prediction
Machine learning was used to predict whether a customer is likely to subscribe based on their demographic and shopping behaviour.

### Target Variable
The target variable was:
- `subscription_status`

The problem was treated as a **binary classification problem** with two possible outcomes:
- Yes – Customer is subscribed
- No – Customer is not subscribed

### Data Preparation
The cleaned customer dataset was used for predictive modelling.

The following steps were performed:
- Selected customer demographic and shopping behaviour features.
- Removed `customer_id` because it is an identifier and does not provide meaningful predictive information.
- Encoded categorical variables using one-hot encoding.
- Split the dataset into training and testing sets using an 80:20 ratio.
- Used stratified splitting to maintain the class distribution.
- Applied feature scaling for Logistic Regression.
- Evaluated model performance using Accuracy, Precision, Recall, and F1-score.

### Models Compared
Three classification models were evaluated:
- Logistic Regression
- Decision Tree
- Random Forest

### Model Performance
| Model | Accuracy | Precision | Recall | F1-Score |
|---|---:|---:|---:|---:|
| Logistic Regression | 84.6% | 68.1% | 81.0% | 74.0% |
| Decision Tree | 84.4% | 67.0% | 82.9% | 74.2% |
| Random Forest | **86.3%** | 66.5% | **99.5%** | **79.7%** |

Random Forest achieved the highest accuracy and F1-score among the three evaluated models and was selected as the best-performing model.

### Important Predictive Features
The Random Forest model identified the following features as important predictors:

- Promo code usage
- Discount application
- Gender
- Previous purchases
- Purchase amount
- Age
- Review rating
- Purchase frequency

These features indicate patterns associated with subscription status and can be used to support customer targeting strategies.

### Business Application
The model can be used as a **customer subscription propensity model** to identify customers who are more likely to subscribe.

High-propensity customers can be prioritized for targeted subscription campaigns and personalized promotional offers. The effectiveness of such campaigns can be further validated using A/B testing.

## 🛠️ Tools & Technologies
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SQL
- PostgreSQL
- Microsoft Power BI
- Power Query
- DAX
- Scikit-learn
- Machine Learning
- Classification
- Feature Engineering
- Model Evaluation


## 🔑 Key Insights
The analysis helps identify:
- Highest-performing products and categories
- Customer groups contributing the most revenue
- Differences in purchasing behaviour across age groups
- Differences in sales contribution across genders
- Purchase frequencies associated with higher sales
- Subscription penetration among customers
- Customer preferences for different payment methods
- Locations with stronger sales performance
- Opportunities for targeted customer campaigns
- Machine learning can be used to identify customers with a higher likelihood of subscription.
- Promotional engagement and discount usage were among the strongest predictive features in the Random Forest model.
- Customer purchase history and demographic characteristics provided additional predictive information.
- Predictive modelling can support targeted subscription campaigns and customer engagement strategies.


## 💡 Business Recommendations
Based on the analysis, businesses can use the findings to support the following decisions:

### 🛍️ Product Strategy
Prioritize high-performing products and optimize inventory based on sales contribution.

### 🎯 Customer Targeting
Create targeted marketing campaigns based on customer demographics and purchasing behaviour.

### 🔄 Customer Retention
Use purchase frequency and subscription behaviour to identify opportunities for repeat purchases and retention campaigns.

### 📢 Marketing Strategy
Design targeted promotions based on customer segments, categories, seasons, and purchasing patterns.

### 📍 Geographic Strategy
Identify high-performing locations and explore opportunities for regional expansion.

### 💳 Payment Optimization
Ensure support for payment methods preferred by customers.

### ⭐ Customer Experience
Monitor ratings and customer feedback to identify opportunities for improving products and services.

### 🤖 Predictive Customer Targeting
Use the subscription prediction model to generate customer propensity scores and prioritize high-probability customers for targeted subscription campaigns.


## 📁 Project Files
- `customer_shopping_behavior.csv` – Original dataset
- `customer_behavior_cleaned.csv` – Cleaned dataset
- `analysis.ipynb` – Python data cleaning and EDA
- `Sql_analysis_queries.txt` – SQL business analysis queries
- `Customer_sales.pbix` – Power BI dashboard
- `Dashboard_Image.png` – Dashboard preview
- `ml/subscription_prediction.ipynb` – Machine learning model for subscription prediction
- `README.md` – Project documentation

---

## 👤 Project Type

**Data Analytics Project**

**End-to-End Workflow:**

`Python → SQL → Power BI`
