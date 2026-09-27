# minorproject-2--SpendDNA
# Spend DNA

**Project Name:** Spend DNA
**Student Name:** Navyashree

## 1. Project Overview

Spend DNA is a data analysis project that analyzes transaction data to understand a person's spending behavior and financial patterns.

The project takes transaction data as input, cleans and processes it, identifies vendors and spending categories, and generates a final Spend DNA report.

## 2. Objectives

The main objectives of this project are:

* Clean and prepare transaction data.
* Extract and standardize vendor names.
* Categorize transactions based on spending patterns.
* Calculate total credits, debits, net amount, and savings rate.
* Analyze monthly spending trends.
* Identify time-of-day spending patterns.
* Detect unusual transactions using Z-score analysis.
* Identify spending archetypes.
* Generate a final Spend DNA report.

## 3. Features

### Feature 1 – Transaction Parser

Cleans the raw transaction data by:

* Converting dates into proper date format.
* Cleaning transaction amounts.
* Standardizing debit and credit values.
* Removing duplicate transactions.
* Checking invalid dates and amounts.

### Feature 2 – Vendor Extractor

Extracts standard vendor names from transaction descriptions.

Examples include:

* Swiggy
* Zomato
* Amazon
* Blinkit
* Zepto
* Uber
* Ola
* Groww
* Netflix
* Spotify
* BigBasket
* DMart
* Jio
* Airtel

ATM transactions are identified as **Cash Withdrawal**.

### Feature 3 – Category Tagger

Transactions are assigned to spending categories such as:

* Food Delivery
* Quick Commerce
* E-commerce
* Subscriptions
* Transport
* Groceries
* Investments
* Utilities
* Cafe
* Restaurants
* Fuel
* Entertainment
* Cash Withdrawal

### Feature 4 – Spending Overview

Calculates:

* Total credits
* Total debits
* Net amount
* Savings rate
* Top spending category
* Category-wise spending

### Feature 5 – Monthly Trend Analysis

Analyzes spending month by month and identifies:

* Monthly spending
* Category-wise monthly spending
* Highest spending month
* Lowest spending month

### Feature 6 – Time-of-Day Patterns

Analyzes when transactions happen during the day.

Transactions are grouped into:

* Morning
* Afternoon
* Evening
* Night

The project also identifies the busiest spending hour.

### Feature 7 – Anomaly Detection

Uses category-based **Z-score analysis** to detect unusual transactions.

Transactions with an absolute Z-score greater than 2 are treated as unusual transactions.

The project displays the top 5 detected anomalies.

### Feature 8 – Spending Archetype Detection

Identifies spending patterns based on predefined rules.

Possible archetypes include:

* The Foodie
* Quick Commerce Junkie
* Shopaholic
* Investor
* Cab Commuter
* YOLO Spender
* Disciplined Saver

### Final Spend DNA Report

The final report combines the major results of the analysis, including:

* Executive summary
* Top spending categories
* Top vendors
* Time-of-day patterns
* Food delivery trends
* Anomalies
* Spending archetypes
* Key insights

## 4. Technologies Used

* **Python**
* **Pandas**
* **NumPy**
* **Jupyter Notebook / Google Colab**
* **CSV Dataset**

## 5. Python Libraries

```python
import pandas as pd
import numpy as np
```

## 6. Dataset

The notebook reads transaction data from:

```text
rahul_transactions.csv
```

The dataset contains transaction information such as:

* Date
* Time
* Amount
* Type
* Description

## 7. How to Run

### Step 1

Install Python and Jupyter Notebook, or open Google Colab.

### Step 2

Upload the notebook:

```text
spendDNA_navya.ipynb
```

### Step 3

Place the transaction CSV file in the same working directory as the notebook.

The expected CSV filename is:

```text
rahul_transactions.csv
```

### Step 4

Open and run the notebook cells from top to bottom.

### Step 5

The notebook will generate the Spend DNA analysis and final report.

## 8. Project Workflow

```text
Transaction CSV
       ↓
Load Dataset
       ↓
Data Cleaning
       ↓
Transaction Parser
       ↓
Vendor Extraction
       ↓
Category Tagging
       ↓
Spending Overview
       ↓
Monthly Trend Analysis
       ↓
Time-of-Day Analysis
       ↓
Anomaly Detection
       ↓
Spending Archetype Detection
       ↓
Final Spend DNA Report
```

## 9. Output
<img width="867" height="1124" alt="image" src="https://github.com/user-attachments/assets/5418321e-8ccb-4717-9c68-0ab3f703574b" />

## 10. Conclusion

Spend DNA provides a structured way to analyze transaction data and understand spending behavior. By combining data cleaning, vendor extraction, category classification, trend analysis, anomaly detection, and spending archetypes, the project generates a consolidated view of transaction patterns.
