# Uncovering Trends in E-Commerce  
### A Data-Driven Approach to Analyzing Online Retail Behavior and Performance

---

## 📌 Overview

This project dives into a real-world e-commerce dataset to uncover deep insights into customer behavior, sales trends, product popularity, seller performance, and much more. By leveraging *Python, **MySQL, and popular **data visualization libraries*, we perform structured analysis using a spectrum of business-oriented SQL queries ranging from beginner to advanced analytics.

---

## 🗂 Project Structure


E-Commerce-Analysis/
│
├── Dataset/
│   ├── customers.csv
│   ├── geolocation.csv
│   ├── order_items.csv
│   ├── orders.csv
│   ├── payments.csv
│   ├── products.csv
│   ├── sellers.csv
│   └── Dataset.txt                  # Dataset source
│
├── Analysis.ipynb                  # Data analysis & visualization notebook
├── csv_to_sql_convetor.ipynb       # Imports CSVs to MySQL tables
├── requirements.txt                # Python dependencies
├── Uncovering Trends in E-Commerce.pdf  # Final report
└── README.md                       # Project documentation


---

## 🔍 Data Analysis Scope

### ▪ Basic Queries
- List all unique customer cities  
- Count orders placed in 2017  
- Total sales by category  
- Percentage of installment payments  
- Customer count by state  

### ▪ Intermediate Queries
- Monthly order count for 2018  
- Average products per order by city  
- Revenue share per category  
- Correlation between product price and frequency  
- Revenue per seller (ranked)  

### ▪ Advanced Queries
- Moving average of order values per customer  
- Cumulative monthly/yearly sales  
- Year-over-year (YoY) growth  
- Customer retention analysis  
- Top 3 spenders per year  

---

## 🛠 Technologies Used

- *Python*: Pandas, Seaborn, Matplotlib  
- *SQL*: MySQL for storage & querying  
- *Jupyter Notebooks*: Data wrangling & visualization  
- *VS Code + Virtual Environment*  
- *XAMPP / Standalone MySQL Server*  

---

## ⚙ Getting Started

### 1. Set Up Virtual Environment (Windows)

bash
# Create environment
python -m venv venv

# Activate
venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt


### 2. MySQL Setup

bash
# Start MySQL service (CMD as Admin)
net start mysql

# OR login manually
mysql -u root -p
# Password: Youre DB password


### 3. Create MySQL Database

sql
CREATE DATABASE ecommerce;
USE ecommerce;


Update database config in both notebooks:

python
db = mysql.connector.connect(
    host='localhost',
    user='root',
    password='Youre DB password',
    database='ecommerce'
)


---

## 📊 Analysis & Visualization Highlights

- Heatmaps showing sales by region  
- Best-selling products and categories  
- Seasonal and monthly sales behavior  
- Revenue growth trends and YoY comparisons  
- Customer segmentation based on activity  
- Seller-wise earnings and performance  

Explore the complete insights in **Analysis.ipynb**  
Summary presented in **Uncovering Trends in E-Commerce.pdf**

---

## 🧾 Dataset Description

| File             | Description                           |
|------------------|---------------------------------------|
| customers.csv  | Customer metadata                     |
| geolocation.csv| Geographic coordinates                |
| orders.csv     | Order history and statuses            |
| order_items.csv| Product-level order data              |
| payments.csv   | Payment types and amounts             |
| products.csv   | Product catalog and categories        |
| sellers.csv    | Seller info and locations             |

> Dataset source: Refer to [Dataset/Dataset.txt](https://www.kaggle.com/datasets/devarajv88/target-dataset?select=products.csv)

---


```