# Customer Behavior Analysis

A full end-to-end data analysis project analyzing customer shopping behavior using Python, SQL, and Power BI.

## Project Overview

This project explores a customer shopping behavior dataset to uncover insights about revenue, customer segments, discount usage, product preferences, and subscription patterns.

## Tools & Technologies

- **Python** (pandas) — data cleaning and feature engineering
- **MySQL** — data storage and analytical queries
- **Power BI** — interactive dashboard and data visualization

## Dataset

Customer shopping behavior dataset containing 3,900 records with fields including:
- Customer demographics (age, gender)
- Purchase details (amount, category, item)
- Behavioral data (subscription status, discount usage, frequency of purchases, review ratings)

## What I Did

### Python (Data Cleaning & Feature Engineering)
- Handled missing values using category-wise median imputation for review ratings
- Standardized column names (lowercase, underscores)
- Created new features:
  - `age_group` — segmented customers into Young Adult, Adult, Middle Age, Senior using quartile binning
  - `purchase_frequency_days` — converted purchase frequency labels into numeric days
- Removed redundant columns after validation
- Exported cleaned data to MySQL database using SQLAlchemy

### SQL (Data Analysis — 10 Questions)
- Total revenue by gender
- High-spending discount users vs average
- Top 5 products by average review rating
- Shipping type vs average purchase amount
- Subscriber vs non-subscriber spend comparison
- Top 5 products by discount rate
- Customer segmentation — New, Returning, Loyal (using CTE)
- Top 3 products per category (using Window Functions)
- Repeat buyer subscription analysis
- Revenue contribution by age group

### Power BI (Dashboard)
- KPI cards: Total Customers, Average Purchase Amount, Average Review Rating
- % of Customers by Subscription Status (donut chart)
- Revenue by Category (bar chart)
- Revenue by Gender (bar chart)
- Revenue by Age Group (horizontal bar chart)
- Average Rating by Product — Top 5 (bar chart)
- Interactive slicers: Subscription Status, Gender, Category, Shipping Type

## Key Insights

- Clothing is the highest revenue-generating category
- Young Adults contribute the most revenue by age group
- 73% of customers are not subscribed — opportunity for growth
- Subscribed customers spend more on average than non-subscribers
- Discount usage does not significantly reduce average spend

## Project Structure

```
customer-behavior-analysis/
│
├── customer_behavior.ipynb        # Python data cleaning & feature engineering
├── customer_behavior.sql.ipynb    # SQL analytical queries
└── customer behavior dashboard.pbix  # Power BI dashboard
```

## How to Run

1. Clone this repository
2. Open `customer_behavior.ipynb` in Jupyter Notebook
3. Run all cells to clean the data and push to MySQL
4. Open `customer_behavior.sql.ipynb` to run SQL queries
5. Open the `.pbix` file in Power BI Desktop to view the dashboard

## Author

**Kartik** — Aspiring Data Analyst
- GitHub: [Karitik](https://github.com/Karitik)
