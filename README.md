# Customer Shopping Behaviour Analysis

## 📌 Project Overview
This project analyzes customer shopping behaviour to understand sales performance, customer characteristics, purchasing patterns, payment preferences, subscription status, and product/category performance.
The analysis follows an end-to-end data analytics workflow:

**Python Data Cleaning & EDA → SQL Business Analysis → Power BI Dashboard**

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


## 📁 Project Files
- `customer_shopping_behavior.csv` – Original dataset
- `customer_behavior_cleaned.csv` – Cleaned dataset
- `analysis.ipynb` – Python data cleaning and EDA
- `Sql_analysis_queries.txt` – SQL business analysis queries
- `Customer_sales.pbix` – Power BI dashboard
- `Dashboard_Image.png` – Dashboard preview
- `README.md` – Project documentation

---

## 👤 Project Type

**Data Analytics Project**

**End-to-End Workflow:**

`Python → SQL → Power BI`
