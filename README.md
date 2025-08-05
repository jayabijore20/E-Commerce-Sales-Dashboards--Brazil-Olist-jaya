# 📊 E-Commerce Sales Dashboard (Brazil – Olist)

**Author**: Jaya Bijore  
**Tool**: Power BI  
**Dataset**: Brazilian E-Commerce Public Dataset by Olist  
**Source**: [Kaggle – Olist Dataset](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

---

## 🧠 Project Objective
To analyze and visualize real-world e-commerce performance metrics using Power BI. The goal is to identify trends, customer behavior, top-performing products, and regional sales performance through interactive visuals and storytelling insights.

---

## 📁 Dataset Files Used
- `olist_orders_dataset.csv`
- `olist_order_items_dataset.csv`
- `olist_order_payments_dataset.csv`
- `olist_order_reviews_dataset.csv`
- `olist_customers_dataset.csv`
- `olist_sellers_dataset.csv`
- `olist_products_dataset.csv`
- `product_category_name_translation.csv`
- `olist_geolocation_dataset.csv`

---

## 🛠️ Power BI Process Summary

### 1. Data Import & Cleaning

- Loaded all `.csv` files into Power BI

- Checked for missing values, date format consistency

- Converted `order_purchase_timestamp` to date format

### 2. Data Modeling

- Created relationships among all 9 tables

- Connected orders → payments, customers, sellers, items, reviews

- Used star schema approach

### 3. DAX Measures Created
- `Total Revenue = SUM(order_payments[payment_value])`

- `Total Orders = DISTINCTCOUNT(order_id)`

- `Average Order Value = [Total Revenue] / [Total Orders]`

- `Average Shipping Duration = AVERAGE(DATEDIFF(order_purchase_timestamp, order_delivered_customer_date, DAY))`

- `Average Review Score = AVERAGE(review_score)`

### 4. Dashboard Design
- Used Cards, Bar Charts, Line Charts, Geo Map, Donut Charts
- 
- Applied dark blue theme with contrasting visuals
- 
- Added slicers: Product Category, Customer State, Review Score, Purchase Date

---

## 📈 Storytelling Insights Report

1)	**RIO DE JANEIRO HAD THE HIGHEST TOTAL REVENUE AT 2.93M BRL**, FOLLOWED BY BELO HORIZONTE AT 1.83M BRL AND CURITIBA AT 1.57M BRL.  

2)	**THESE 3 CITIES ACCOUNTED FOR OVER 40% OF THE TOTAL SALES REVENUE**, OUT OF 15.42M BRL GENERATED ACROSS BRAZIL.

  
3)	**NOVEMBER HAD THE HIGHEST MONTHLY REVENUE, EXCEEDING 2M BRL**, FOLLOWED BY JULY. JANUARY SHOWED A NOTABLE DIP IN SALES.  

4)	**CREDIT CARDS ACCOUNTED FOR 78.47% OF TOTAL TRANSACTIONS**, WHILE BOLETO COVERED 17.96% — INDICATING A STRONG PREFERENCE FOR DIGITAL PAYMENTS.  


5)	**"BED_BATH_TABLE" AND "HEALTH_BEAUTY" WERE THE HIGHEST-GROSSING PRODUCT CATEGORIES**, EACH CONTRIBUTING OVER 1.5M BRL IN SALES.

  
6)	**CUSTOMER FEEDBACK INDICATES HIGH SATISFACTION**, WITH 70% OF ORDERS RECEIVING A REVIEW SCORE OF 4 OR 5.  


7) **AVERAGE ORDER VALUE WAS 160 BRL**, WHILE AVERAGE DELIVERY TIME STOOD AT 12.5 DAYS — SUGGESTING ROOM FOR IMPROVEMENT IN SHIPPING SPEED.

---

## 📸 Sample Dashboard Screenshot

Included in GitHub repo as: `ecommerce sales dashboard pdf’
-Report of dashbords
- Raw data file

---

## 📬 Contact

**Jaya Bijore**  

[GitHub](https://github.com/jayabijore20)

