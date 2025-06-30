#  Uncovering Trends in E-Commerce  
### *A Data-Driven Approach to Analyzing Online Retail Behavior and Performance*

---

## 📌 Overview

This project explores a real-world e-commerce dataset to derive actionable insights into:

- 🛍️ Customer behavior  
- 📦 Product popularity  
- 💰 Seller performance  
- 📈 Sales trends

By leveraging **Python**, **MySQL**, and **data visualization libraries**, we dive into beginner to advanced SQL analytics, visual storytelling, and interactive dashboards.

---

## 🗂️ Project Structure

```

E-Commerce-Analysis/
│
├── Dataset/
│   ├── customers.csv
│   ├── geolocation.csv
│   ├── order\_items.csv
│   ├── orders.csv
│   ├── payments.csv
│   ├── products.csv
│   ├── sellers.csv
│   └── Dataset.txt                  # Dataset source
│
├── Analysis.ipynb                  # Data analysis & visualization notebook
├── csv\_to\_sql\_convetor.ipynb       # Imports CSVs to MySQL tables
├── requirements.txt                # Python dependencies
├── Uncovering Trends in E-Commerce.pdf  # Final report
└── README.md                       # Project documentation

````

---

## 🔍 Data Analysis Scope

### ✅ Basic Queries
- 🌆 List all unique customer cities  
- 📅 Count of orders placed in 2017  
- 🏷️ Total sales by category  
- 💳 Percentage of installment payments  
- 🧾 Customer count by state  

### 📊 Intermediate Queries
- 📆 Monthly order count for 2018  
- 🛒 Average products per order by city  
- 📁 Revenue share per category  
- 💡 Correlation: product price vs frequency  
- 🏆 Revenue per seller (ranked)  

### 🔬 Advanced Queries
- 📈 Moving average of order values per customer  
- 📅 Cumulative monthly/yearly sales  
- 📊 Year-over-year (YoY) growth  
- 🔁 Customer retention metrics  
- 💸 Top 3 spenders per year  

---

## 🛠️ Technologies Used

- **Python**: `Pandas`, `Seaborn`, `Matplotlib`  
- **SQL**: MySQL (Structured Query Language)  
- **Notebook**: Jupyter for visualization  
- **Environment**: VS Code + Virtual Environment  
- **Database**: XAMPP / MySQL Server  

---

## ⚙️ Getting Started

### 1️⃣ Set Up Python Virtual Environment (Windows)

```bash
# Create environment
python -m venv venv

# Activate environment
venv\Scripts\activate

# Install required packages
pip install -r requirements.txt
````

### 2️⃣ MySQL Setup

```bash
# Start MySQL service (Admin CMD)
net start mysql

# OR login manually
mysql -u root -p
# Password: <Your DB password>
```

### 3️⃣ Create MySQL Database

```sql
CREATE DATABASE ecommerce;
USE ecommerce;
```

Update DB config inside both notebooks:

```python
db = mysql.connector.connect(
    host='localhost',
    user='root',
    password='Your DB password',
    database='ecommerce'
)
```

---

## 📊 Analysis & Visualization Highlights

* 📍 Heatmaps of sales by region
* 🏆 Best-selling products & categories
* 🗓️ Monthly & seasonal sales trends
* 📈 YoY revenue comparisons
* 👥 Customer segmentation by activity
* 🤝 Seller-wise performance and revenue

👉 Full analysis: `Analysis.ipynb`
📄 Final summary: `Uncovering Trends in E-Commerce.pdf`

---

## 📁 Dataset Description

| File              | Description                         |
| ----------------- | ----------------------------------- |
| `customers.csv`   | Customer metadata                   |
| `geolocation.csv` | Customer coordinates (Lat, Long)    |
| `orders.csv`      | Order status & timestamps           |
| `order_items.csv` | Detailed product-level order info   |
| `payments.csv`    | Payment types & transaction amounts |
| `products.csv`    | Product info & categories           |
| `sellers.csv`     | Seller info and location            |

🔗 **Dataset Source**: Refer to [`Dataset.txt`](https://www.kaggle.com/datasets/devarajv88/target-dataset?select=products.csv)

---

## 🔗 Clone This Repository

```bash
git clone https://github.com/Jasika-Kumari/E-Commerce-Analytics.git
```

---

