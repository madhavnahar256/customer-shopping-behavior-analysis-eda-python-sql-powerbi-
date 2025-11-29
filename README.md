# customer-shopping-behavior-analysis-eda-python-sql-powerbi-
📘 Customer Shopping Behavior Analysis — README

A deep-dive analysis into how customers shop, what they buy, and how their demographics influence purchasing behavior. This project blends Python (EDA), SQL business queries, and a Power BI dashboard to convert raw transactional data into clear, decision-ready insights.

## Project Overview

This project analyzes 3,900+ customer transactions to uncover:
Spending patterns
Category-wise performance
Subscription influence on purchasing
Behavior across age groups
Revenue and sales drivers
The goal is to help businesses make data-driven decisions in product strategy, pricing, customer retention, and marketing.

###🗂️ Dataset Summary
Rows: 3,900
Columns: 18
Key Features:
Demographics → Age, Gender, Subscription Status
Purchase Info → Category, Purchase Amount, Season, Size, Color
Behavior Data → Discount Applied, Previous Purchases, Shipping Type
Ratings → Review Rating (37 missing values fixed during EDA)

####🔍 Exploratory Data Analysis (Python)
Performed using pandas, numpy, matplotlib, and seaborn.
✔ Cleaned and prepared dataset
✔ Handled missing values (median imputation by category)
✔ Standardized column names
✔ Engineered new features:
                           age_group (young adult, middle-aged, adult, senior)
                          purchase_frequency_days
✔ Dropped redundant fields (ex: promo code vs discount applied)
✔ Loaded cleaned data into PostgreSQL for analytics

#####🧠 SQL Business Analysis
Using PostgreSQL, multiple business questions were answered:
Revenue comparison by gender, age group, subscription status
Most profitable product categories
Discount-dependent products
High-spending discount users
Top-rated and top-selling products
Customer segmentation → New, Returning, Loyal
Repeat buyers and their likelihood of subscription
Shipping type analysis → Standard vs Express

#####📊 Power BI Dashboard
The final dashboard brings insights alive through:
Key Metrics
Avg Purchase Amount: $59.76
Avg Review Rating: 3.75
Total Customers: 3.9K
Major Visuals
Revenue by category
Sales by category
Revenue & sales by age group
Subscription distribution (Yes – 27%, No – 73%)
Filters for gender, subscription, and category
The dashboard acts like a decision-lens, showing how different customer types contribute to business outcomes.

######💡 Business Insights
Clothing is the highest revenue generator (104K).
Young Adults contribute the highest sales volume.
73% of customers are non-subscribers → opportunity for subscription campaigns.
Subscribers spend more on average → promote loyalty and exclusive offers.
Accessories and Footwear show strong cross-sell potential.
Express shipping users tend to spend more → upsell opportunity.

###### Technologies Used
Python (EDA)
Pandas, NumPy, Matplotlib, Seaborn
PostgreSQL (Business queries)
Power BI (Dashboard visualization)
Git & GitHub (Version control)

#######📁 Project Structure
|-- EDA/
|   |-- Customer_Shopping_Behavior_Analysis.ipynb
|
|-- Dashboard/
|   |-- PowerBI_Dashboard.png
|
|-- Reports/
|   |-- Project_Report.pdf
|
|-- README.md
|-- data.csv

########📥 How to Use the Project
Download the dataset
Open the EDA notebook
Explore insights with Python
Run SQL queries for deeper business analytics
View the interactive Power BI dashboard
