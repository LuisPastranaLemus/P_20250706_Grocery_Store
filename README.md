# 🧭 Project Analysis
This project explores and analyzes the Grocery Inventory Dataset, aiming to extract actionable insights for improving inventory management, sales performance, supplier efficiency, and customer satisfaction in a retail grocery environment.

---

## 🔍 Project Overview (P-20250706_Grocery_Store)

This project focuses on analyzing a comprehensive grocery inventory dataset to uncover key business insights that support better decision-making in a retail environment. Through data exploration and visualization, it is aimed to identify product trends, optimize inventory levels, evaluate supplier reliability, and understand customer behavior. The analysis supports strategic actions such as improving stock management, increasing sales, minimizing losses, and enhancing customer satisfaction.

This analysis seeks to "empower grocery managers with data-driven decisions"

Key questions:

- Identify high- and low-performing products in terms of sales, margin, and turnover.
- Detect stockouts and overstock situations to optimize inventory levels.
- Evaluate supplier performance based on delivery times and order accuracy.
- Understand customer purchasing behavior and product demand trends.
- Propose business strategies to increase profitability and operational efficiency.

Project Info explanation

__Note__: key info

---

## 🧮 Data Dictionary

This project has 6 different tables.

- `products.csv` (Product information details)
    `product_id`:	  Unique identifier for each product.
    `product_name`:   Name of the product (brand + category).
    `category`:       Product category (e.g., Dairy, Snacks).
    `supplier_id`:    Foreign key linking to the supplier.
    `unit_cost`:	  Cost price of the product (wholesale).
    `status`:	      Availability: Active, Backordered, or Discontinued.
    `brand`:	      Brand or manufacturer name.
    `list_price`:     Retail price per unit.

- `suppliers.csv` (Suppliers information details)
    `supplier_id`:	    Unique ID for each supplier.
    `supplier_name`:	Company or supplier name.
    `lead_time_days`:   Average delivery time in days.
    `contact_info`:	    Phone or other contact information.
    `rating`:	        Supplier performance rating (scale 1–5).

- `inventory.csv` (Inventory information details)
    `inventory_id`:	    Unique ID for inventory record.
    `date`:     	    Date of inventory record.
    `product_id`:	    Foreign key to products table.
    `beginning_stock`:	Units in stock at start of the day.
    `received`:     	Units received during the day.
    `sold`:         	Units sold during the day.
    `ending_stock`:	    Units remaining at the end of the day.
    `warehouse_location`:	Location or region of the warehouse.

- `transactions.csv` (Transactions information details)
    - `transaction_id`:	Unique ID for the sales transaction.
    - `date`:	        Date of transaction.
    - `product_id`: 	Product sold (linked to products).
    - `units_sold`:  	Quantity sold in transaction.
    - `customer_id`:	Buying customer (linked to customers).
    - `employee_id`:	Salesperson who handled the transaction.
    - `list_price`: 	Unit price at time of sale.
    - `sales_amount`:	Total transaction amount (units × price).

- `customers.csv` (Customers information details)
    - `customer_id`:    Unique customer identifier.
    - `customer_name`:	Full name of the customer.
    - `join_date`:  	When the customer was registered.
    - `total_spent`:	Total historical spend.
    - `frequency`:		Number of visits or transactions.
    - `segment`:    	Customer segment (e.g., Frequent, High Value).

- `salesforce.csv` (Salesforce information details)
    - `employee_id`:    Unique salesperson ID.
    - `employee_name`:	Name of the salesperson.
    - `region`:     	Assigned sales region.
    - `total_sales`:	Aggregate value of sales handled.
    - `effectiveness`:	Success rate of transactions closed.

---

## 📂 Project Structure

```bash
├── data/
│   ├── raw/              # Original dataset(s) in CSV format
│   ├── interim/          # Intermediate cleaned versions
│   └── processed/        # Final, ready-to-analyze dataset
│
├── notebooks/
│   ├── 01_cleaning.ipynb                        ← Custom cleaning 
│   ├── 02_feature_engineering.ipynb             ← Custom feature engineering
│   ├── 03_eda_and_insights.ipynb                ← Exploratory Data Analysis & visual storytelling
│   └── 04-sda_hypotheses.ipynb                  ← Business insights and hypothesis testing
│
├── src/
│   ├── init.py              # Initialization for reusable functions
│   ├── data_cleaning.py     # Data cleaning and preprocessing functions
│   ├── data_loader.py       # Loader for raw datasets
│   ├── eda.py               # Exploratory data analysis functions
│   ├── features.py          # Creation and transformation functions for new variables to support modeling and EDA
│   └── utils.py             # General utility functions for reusable helpers
│
├── outputs/
│   └── figures/          # Generated plots and visuals
│
├── requirements/
│   └── requirements.txt      # Required Python packages
│
├── .gitignore            # Files and folders to be ignored by Git
└── README.md             # This file
```
---

🛠️ Tools & Libraries

- Python 3.12
- os, pathlib, sys, pandas, NumPy, Matplotlib, plotly, seaborn, IPython.display, scipy.stats, streamlit
- Jupyter Notebook
- Git & GitHub for version control
- Streamlit

---

## 📌 Notes

This project is part of a personal learning portfolio focused on developing strong skills in data analysis, statistical thinking, and communication of insights. Constructive feedback is welcome.

---

## 👤 Author   
##### Luis Sergio Pastrana Lemus   
##### Engineer pivoting into Data Science | Passionate about insights, structure, and solving real-world problems with data.   
##### [GitHub Profile](https://github.com/LuisPastranaLemus)   
##### 📍 Querétaro, México     
##### 📧 Contact: luis.pastrana.lemus@engineer.com   
---

