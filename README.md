**Customer Shopping Behaviour Analysis**

📌Project Overview:

This project analyzes customer shopping behaviour to understand sales performance, customer characteristics, purchasing patterns, payment preferences, subscription status, and product/category performance.
The analysis follows an end-to-end data analytics workflow, starting with **data cleaning and exploratory data analysis using Python**, followed by **SQL-based business analysis**, and finally transforming the findings into an interactive **Microsoft Power BI dashboard**.

Problem Statement:
Businesses collect large amounts of customer purchase data, but raw transaction data alone does not clearly reveal customer purchasing patterns, product performance, demographic trends, or sales opportunities. The objective of this project is to analyze customer shopping behaviour and transform the data into actionable insights that can support decisions related to products, categories, customer segments, purchasing frequency, subscriptions, payment methods, and geographic sales performance.


🎯 Business Objectives:

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

📊 Dataset:
Kaggle Dataset:

Rows: 3,900 customer records

Key fields: Customer ID, Age, Gender, Item Purchased, Category, Purchase Amount, Previous Purchases, Frequency of Purchases, Payment Method, Location, Subscription Status, Discount Applied,Promo Code, Season, Review Rating, Shipping Type, and related attributes.

**Workflow of Analytics**

**1. Data Cleaning & Preparation**:
Python was used to inspect and prepare the raw dataset before performing analysis.

Activities performed:
1)Loaded and inspected the dataset.
2)Checked dataset structure and data types.
3)Identified missing values.
4)Checked duplicate records.
5)Examined categorical and numerical columns.
6)Handled data quality issues.
7)Converted columns into appropriate data types.
8)Created additional analytical fields.
9)Prepared the cleaned dataset for further analysis.
10)Additional fields created:
   -age_group
   -purchase_frequency_days
These fields were later used for customer segmentation and purchasing behaviour analysis.

**2. Exploratory Data Analysis (EDA)**
Exploratory Data Analysis was performed using Python to understand the structure and behaviour of the data before building the final dashboard.

EDA included:
Univariate analysis
Categorical variable analysis
Numerical variable analysis
Distribution analysis
Customer demographic analysis
Purchase behaviour analysis
Sales analysis
Relationship analysis between important variables
Python Libraries Used
Pandas
NumPy
Matplotlib
Seaborn

EDA helped identify patterns and relationships that were later converted into business questions and dashboard visuals.

**3. SQL Business Analysis**
SQL was used to perform business-focused analysis on the cleaned customer dataset and answer key business questions.

The analysis covered:

Revenue comparison across customer genders.
Customers who used discounts but spent above average.
Top products based on average review ratings.
Comparison of spending across shipping types.
Spending behaviour of subscribed vs. non-subscribed customers.
Products with the highest discount usage.
Customer segmentation based on previous purchases.
Top products within each category.
Relationship between repeat purchases and subscription status.
Revenue contribution across different age groups.

The SQL analysis helped convert raw customer data into specific business questions, measurable metrics, and actionable insights.

**4. Power BI Dashboard & Visualization**
The final analysis was transformed into an interactive Power BI dashboard to present the major findings in a clear and business-friendly format.

KPI Metrics
Total Customers
Total Sales
Average Transaction
Average Rating
Dashboard Visualizations
Top 10 Products by Sales
Sales by Category
Customer Subscription Status
Sales by Purchase Frequency
Sales by Gender
Sales by Age Group
Sales by Location
Payment Method Distribution

**🛠️ Tools & Technologies**

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SQL / PostgreSQL
- Microsoft Power BI
- Power Query
- DAX


**Key Insights**
The analysis helps identify:

-Highest-performing products and categories.
-Customer groups contributing the most revenue.
-Differences in purchasing behaviour across age groups.
-Differences in sales contribution across genders.
-Purchase frequencies associated with higher sales.
-Subscription penetration among customers.
-Customer preferences for different payment methods.
-Locations with stronger sales performance.
-Opportunities for targeted customer campaigns.

**Business Recommendations**
Based on the analysis, businesses can use the findings to:

🛍️ Product Strategy
Prioritize high-performing products and optimize inventory based on sales contribution.

🎯 Customer Targeting
Create targeted marketing campaigns based on customer demographics and purchasing behaviour.

🔄 Customer Retention

Use purchase frequency and subscription behaviour to identify opportunities for repeat purchases and retention campaigns.
📢 Marketing Strategy

Design targeted promotions based on customer segments, categories, seasons, and purchasing patterns.
📍 Geographic Strategy

Identify high-performing locations and explore opportunities for regional expansion.
💳 Payment Optimization

Ensure support for payment methods preferred by customers.
⭐ Customer Experience

Monitor ratings and customer feedback to identify opportunities for improving products and services.



