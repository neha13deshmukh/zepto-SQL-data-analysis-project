# 🛒 Zepto Inventory Data Analysis (MySQL Project)

## 📌 Project Overview

This project focuses on analyzing a real-world e-commerce inventory dataset using MySQL.

The objective was to simulate how data analysts work with raw data — starting from data exploration, performing cleaning, and finally deriving meaningful business insights using SQL queries.

---

## 📁 Dataset Overview

The dataset used in this project was sourced from Kaggle and is based on product listings scraped from Zepto’s platform.

It represents a real-world e-commerce inventory dataset, including product details such as pricing, discounts, stock availability, and categories. The structure closely resembles data used in actual retail and quick-commerce systems.

### 🔹 Columns Used:

* **name** – Product name
* **category** – Product category
* **mrp** – Maximum Retail Price
* **discountPercent** – Discount applied
* **discountedSellingPrice** – Final selling price
* **availableQuantity** – Available stock
* **weightInGms** – Product weight
* **outOfStock** – Stock availability (1 = Out of stock, 0 = In stock)
* **quantity** – Units per product

---

## ⚙️ Tools & Technologies

* **MySQL** – Data analysis
* **SQL** – Query writing (EDA, Cleaning, Analysis)
* **GitHub** – Project hosting

---

## 🔧 Project Workflow

### 1️⃣ Database Setup

* Created a MySQL database
* Imported dataset using table import feature

```sql
CREATE DATABASE zepto_Project;
USE zepto_Project;
```

---

### 2️⃣ Data Exploration (EDA)

Performed initial analysis to understand the dataset:

* Counted total number of records
* Viewed sample data
* Checked for NULL values
* Identified unique product categories
* Analyzed stock availability (in-stock vs out-of-stock)
* Detected duplicate product names (multiple SKUs)

---

### 3️⃣ Data Cleaning

Cleaned and prepared data for accurate analysis:

* Identified products with zero price
* Removed invalid records where MRP = 0
* Handled price conversion carefully (validated paise vs rupees issue)
* Verified data using MIN/MAX checks

---

### 4️⃣ Data Analysis (Business Insights)

* Found top 10 best-value products based on discount percentage
* Identified high-MRP products that are currently out of stock
* Estimated potential revenue for each product category
* Filtered expensive products (MRP > ₹500) with minimal discount
* Ranked top 5 categories offering highest average discounts
* Calculated price per gram to identify value-for-money products
* Grouped products into Low, Medium, and Bulk categories based on weight
* Measured total inventory weight per category

---

## 🧠 Key Learnings

* Importance of validating data before transformation
* Handling real-world issues like NULL values and incorrect assumptions
* Debugging SQL queries when results are empty
* Writing queries based on business problems, not just syntax

---

## 🚀 How to Run This Project

1. Create a MySQL database
2. Import the dataset into a table
3. Run queries step-by-step:

   * Data Exploration
   * Data Cleaning
   * Data Analysis

---

## 💡 Conclusion

This project helped me strengthen my SQL skills and understand how to work with real-world datasets.

I focused not only on writing queries but also on interpreting results to generate meaningful business insights.

---

## 👩‍💻 About Me

I am an aspiring Data Analyst skilled in SQL, Power BI, and data analysis.

Currently building projects to improve problem-solving skills and prepare for data analyst roles.

---

