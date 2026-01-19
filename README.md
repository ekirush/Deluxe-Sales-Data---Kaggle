# Deluxe Sales Data Analysis (2019-2020)

## 📌 Introduction
This repository contains an exploratory data analysis (EDA) of the "Deluxe" online store sales dataset. The goal of this project was to clean raw sales data, engineer relevant features (profit, margins, date granularity), and visualize key performance indicators to uncover trends in revenue, customer behavior, and operational efficiency.

## 📂 Data Overview
The dataset consists of **1000 rows** and **10 columns** covering sales transactions.
* **Time Period:** 2019 - 2020
* **Key Features:** `Country`, `Category`, `Revenue`, `Cost`, `Sales Rep`, `Device Type`, and `Customer Name`.
* **Tech Stack:** Python, Pandas, Seaborn, Matplotlib.

## 🛠️ Methodology
1.  **Data Cleaning:**
    * Converted `date` to datetime objects.
    * Cleaned currency strings (removed commas) and converted to float.
    * Checked for duplicates (0 found) and null values.
2.  **Feature Engineering:**
    * Calculated `Profit` = Revenue - Cost.
    * Calculated `Profit Margin %`.
    * Extracted `Month`, `Year`, and `Weekday` for time-series analysis.
3.  **Visualization:**
    * Used Seaborn for statistical graphics (Distributions, Boxplots, Heatmaps).

## 📊 Key Results

### 1. Sales Trends
* **Seasonality:** Sales exhibit a bi-annual peak structure, maximizing in **June** and **December**. February and November show significant dips in revenue.
* **Category Performance:** **Clothing** is the top-performing category (~17.6M), followed by **Games**.

### 2. Market & Device Analysis
* **Geography:** **Portugal** is the primary market, significantly outperforming France and Sweden.
* **Platform:** Transactions are overwhelmingly dominated by **PC users**, suggesting a B2B nature or complex purchasing journey that discourages mobile use.

### 3. Customer Loyalty
* **Retention:** The dataset shows an exceptionally high ratio of **Repeat Buyers** vs. One-time buyers. The business has high customer stickiness but appears to lack a strong new customer acquisition channel.

### 4. Sales Team
* **Pareto Principle:** A small group of sales representatives (e.g., Corene Shrier) drives a disproportionate amount of revenue.

## 🚀 Recommendations
Based on the data analysis, the following actions are recommended:
1.  **Customer Acquisition:** Launch targeted campaigns to attract *new* customers, as the current base is stagnant (albeit loyal).
2.  **Regional Expansion:** Analyze the "Portugal Playbook" to understand why it succeeds and replicate those strategies in low-performing regions like Belgium and Austria.
3.  **Inventory Planning:** Align inventory stocking with the identified June/December peaks to prevent stockouts in high-velocity categories like Clothing.
4.  **Desktop Optimization:** Prioritize desktop UI/UX improvements over mobile app development, given the device usage data.

---
*Analysis generated via Python (Pandas/Seaborn).*
