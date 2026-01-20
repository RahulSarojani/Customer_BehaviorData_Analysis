**End-to-End Data Analytics Portfolio Project**
Analyzing 3,900 customer transactions to uncover shopping patterns, customer segments, product preferences, and subscription insights.
| Python + SQL + Power BI | EDA on 3,900 transactions: spending patterns, customer segments, discounts &amp; subscriptions
---

## Project Overview

This project analyzes real-world customer shopping behavior using transactional data.

**Objective**:
To generate actionable business insights related to revenue drivers, discount usage, customer loyalty, and subscription adoption using a complete analytics workflow.

This is my **first complete end-to-end data analytics portfolio project**, covering data cleaning, analysis, and visualization.

---

## Business Problem

A retail business wants to better understand:

* Who their most valuable customers are
* Which products and categories drive revenue
* How discounts and subscriptions affect spending
* Opportunities to improve loyalty and conversion

The goal is to support **data-driven decision-making** for marketing, pricing, and customer retention strategies.

---

## Dataset

* **Source**: Customer Shopping Trends Dataset (Kaggle)
* **Records**: 3,900 transactions
* **Features**: 18 columns

### Key Attributes

* **Customer Demographics**: customer_id, age, gender, location, subscription_status
* **Purchase Details**: item_purchased, category, purchase_amount_usd, season, size, color
* **Behavioral Data**: review_rating, discount_applied, promo_code_used, previous_purchases, payment_method, frequency_of_purchases, shipping_type

### Data Quality

* Missing values: 37 records in `review_rating`
* Treatment: Imputed using **median review rating per product category**

---

## Tools & Technologies

* **Python**: Pandas, NumPy (data cleaning, EDA, feature engineering)
* **MySQL**: Data storage and analytical SQL queries
* **Power BI**: Interactive dashboards and visual storytelling
* **Development Environment**: VS Code (primary), Google Colab (initial attempt)
* **Operating Systems**: macOS (initial), Windows (final execution)

---

## Project Workflow

### 1. Data Understanding & Cleaning (Python)

* Loaded dataset using Pandas
* Performed structural and statistical exploration
* Handled missing values in `review_rating`
* Standardized column names to `snake_case`
* Feature engineering:

  * Created `age_group` (Young Adult, Adult, Middle-aged, Senior)
* Identified and removed redundant columns

> Initial cleaning attempts were done in **Google Colab**, but column renaming caused confusion. The workflow was shifted to **VS Code** for better control and debugging.

---

### 2. Database Loading (MySQL)

* Exported cleaned dataset from Python
* Imported data into MySQL for structured querying
* Used SQL for business-focused analysis

---

### 3. SQL Analysis – Business Questions

Key questions addressed:

* Revenue distribution by gender and age group
* Subscriber vs non-subscriber performance
* High-spending customers using discounts
* Products most dependent on discounts
* Top products by average review rating
* Shipping type vs average purchase value
* Customer segmentation (New, Returning, Loyal)
* Repeat purchases and subscription correlation

---

### 4. Visualization & Dashboard (Power BI)

* Connected Power BI to MySQL database (local Windows setup)
* Designed an interactive dashboard with:

  * KPI cards
  * Bar and pie charts
  * Tables for product-level insights

**Dashboard Highlights**:

* Subscription split (Yes vs No)
* Revenue by age group and category
* Gender-based revenue comparison
* Shipping type distribution
* Top products by sales and ratings

---

## Challenges Faced & Learnings

* **macOS Limitation**: Power BI Desktop is not supported on macOS

  * Python and MySQL work completed on Mac
  * Switched to **Windows** to build Power BI dashboards

* **MySQL to Power BI Connectivity**:

  * Attempted AWS RDS and IP whitelisting approaches
  * Faced connectivity issues (still learning and experimenting)
  * Completed final dashboard using local MySQL on Windows

* **Tooling Workflow Adjustment**:

  * Google Colab caused confusion during early cleaning
  * Migrated to VS Code for a more stable development workflow

These challenges strengthened my understanding of **cross-platform planning**, **tool limitations**, and **practical problem-solving**.

---

## Key Insights

* Male customers generate nearly **2× more revenue** than females
* Loyal customers dominate the dataset, indicating strong repeat behavior
* Young Adults contribute the highest revenue share
* Express shipping users spend slightly more per transaction
* Hats, Sneakers, and Coats are highly discount-dependent
* Subscription adoption is only ~27% despite high repeat purchases
* Average purchase value: ~$59.76
* Average product rating: ~3.75

---

## Business Recommendations

* Convert repeat buyers into subscribers through targeted campaigns
* Strengthen loyalty programs for high-frequency customers
* Reassess discount strategies for margin-sensitive products
* Promote top-rated and high-performing products in marketing
* Focus campaigns on high-revenue segments such as Young Adults

---

## How to Run This Project

1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/customer-shopping-analysis.git
cd customer-shopping-analysis
```

2. Run Python notebook

* Open the Jupyter notebook or Python script
* Execute data cleaning and feature engineering steps

3. Load data into MySQL

* Create a database and table
* Import the cleaned CSV file

4. Execute SQL queries

* Use the provided SQL script to generate insights

5. Open Power BI Dashboard

* Connect Power BI to the MySQL database (Windows)
* Load visuals and interact with the dashboard

---

## Project Status

Completed ✔️
Future improvements:

* Cloud-based MySQL → Power BI connection
* Advanced customer segmentation
* Predictive modeling for customer lifetime value

---

## Author

**Rahul Patil**
Aspiring Data Analyst | Data Science for Social Impact

---

If you are a recruiter or hiring manager, this project demonstrates my ability to handle an **end-to-end analytics workflow**, overcome real-world constraints, and translate data into actionable business insights.
