# Ecommerce_Sales_Data_2024_2025_PowerBI
Power BI analysing Ecommerce_Sales_Data_2024_2025 analysis
# 📊 Ecommerce Sales Data Analysis Dashboard

## 📌 Project Overview

This project focuses on cleaning, transforming, and analyzing an ecommerce dataset using Excel and visualizing insights using Power BI.

The goal is to identify trends in sales, profit, customer behavior, and regional performance through an interactive dashboard.

---

## 🧹 Data Cleaning (Excel)

### 1. Data Cleaning

* No duplicate records were found.
* Inconsistencies in:

  * Customer Name
  * Product Name
  * Sub-Category
* Fixed using:

  * Find & Replace
  * `TRIM()` – removes extra spaces
  * `PROPER()` – capitalizes first letter of each word

---

### 2. Data Imputation

#### Handling Missing Values

* **Sub-Category:**

  ```excel
  =IF(ISBLANK(cell),"Unknown",cell)
  ```

* **Payment Mode:**

  ```excel
  =IF(ISBLANK(cell),"Cash",cell)
  ```

---

#### Numerical Columns

* **Quantity:**

  ```excel
  =IF(ISBLANK(cell),AVERAGEIF(range,criteria,average_range),cell)
  ```

  ```excel
  =ROUND(N,0)
  ```

* **Unit Price:**

  ```excel
  =IF(ISBLANK(Unit_Price), Total_Amount / (Qty*(1-Discount)), Unit_Price)
  ```

---

### 3. Feature Engineering

* Extracted:

  * Order Month
  * Order Year
* Done using delimiter-based splitting from Order Date.

---

### 4. Data Preparation

* Sorted Order ID in ascending order
* Applied filtering for validation

---

### 5. Descriptive Statistics

Using Excel Data Analysis ToolPak:

* Sum
* Average
* Median
* Mode
* Skewness

Applied on:

* Quantity
* Unit Price
* Discount
* Sales
* Profit

---

## 📊 Data Visualization (Power BI)

An interactive dashboard was created to communicate key business insights.

### 🔢 Key Metrics

* Total Orders
* Total Sales
* Total Profit
* Total Revenue
* Total Discount
* Year-to-Date (YTD)

---

### 📈 Visualizations Used

* Clustered Bar Chart → Orders by Category & Region
* Donut Chart → Profit by Category
* Stacked Area Chart → Sales & Profit by Month
* Treemap → Sales by City, Region, Quantity
* Line + Stacked Column Chart → Revenue & Sales Trend
* Funnel Chart → Discount by Category

---

### 🎛 Features

* Filters and slicers
* Drill-down functionality (Treemap)
* Interactive layout
* Clear titles, labels, and legends

---

## 📤 Output

* Final dashboard exported as PDF:

  * `output/ecommerce_dashboard.pdf`

---

## 🛠 Tools Used

* Microsoft Excel
* Power BI

---

## 🚀 How to Use

1. Download the dataset from `/data`
2. Review cleaning steps in `/scripts`
3. Open `.pbix` file in Power BI
4. Explore the dashboard or view exported PDF

---
