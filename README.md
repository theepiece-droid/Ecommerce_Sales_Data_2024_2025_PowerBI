## 📊 Ecommerce Sales Data Analysis and insights using Excel and Power BI

## 🏷️ Project Overview

- **Domain:** Ecommerce – Profit & Revenue Analysis  
- **Business Context:** Finance  

## 🛠️ Tech Stack

- **Tools:** Power BI, Microsoft Excel  
- **Language:** DAX (Data Analysis Expressions)  
- **Technologies:** Power Query, Data Modeling  

## 📊 Key Focus

- Financial data analysis and reporting  
- Profitability and revenue insights  
- Interactive dashboard development using Power BI  


## 🧹 Data Pre-processing (Excel)

### Data Cleaning

* Verified dataset integrity and confirmed absence of duplicate records.
* Standardized textual inconsistencies in **Customer Name**, **Product Name**, and **Sub-Category** using:

  * Find & Replace
  * `TRIM()` for whitespace removal
  * `PROPER()` for consistent capitalization

---

### Missing Value Treatment

#### Categorical Variables

* Addressed null values in **Sub-Category** and **Payment Mode** using conditional imputation:

  * Replaced missing entries with "Unknown" and "Cash" respectively using `IF(ISBLANK())`.

#### Numerical Variables

* **Quantity:**

  * Imputed using conditional mean (`AVERAGEIF()`) based on relevant criteria
  * Standardized values using `ROUND()`

* **Unit Price:**

  * Derived missing values using a business rule:

    ```
    Unit Price = Total Amount / (Quantity × (1 - Discount))
    ```

---

### Feature Engineering

* Extracted **Order Month** and **Order Year** from the Order Date column to enable time-series analysis.

---

### Data Structuring & Validation

* Sorted dataset by **Order ID** in ascending order.
* Applied filtering techniques to validate cleaned data and ensure consistency.

---

### Statistical Analysis

* Leveraged Excel’s **Data Analysis ToolPak** to compute:

  * Sum, Mean, Median, Mode, Skewness
* Applied across key variables:

  * Quantity, Unit Price, Discount, Sales, Profit
---
## 📂 Dataset Attributes

This dataset contains summarized eCommerce sales metrics used for financial analysis and dashboard reporting.

### 🧾 Columns Description

| Column Name | Description |
|------------|------------|
| Quantity | Number of units sold |
| Unit Price | Price per unit of product |
| Discount | Discount applied on products |
| Sales | Total sales value generated |
| Profit | Profit earned after discount and cost adjustments |

### 📊 Statistical Metrics Included

| Metric | Description |
|--------|------------|
| Mean | Average value of each metric |
| Median | Middle value of the dataset |
| Mode | Most frequently occurring value |
| Standard Error | Measure of data variability |

### 📈 Usage in Project

| Area | Details |
|------|--------|
| Analysis | Financial performance analysis |
| Insights | Sales trends and profitability evaluation |
| Power BI | Used for DAX measures and KPI creation |

### 🧹 Data Characteristics

| Feature | Description |
|--------|------------|
| Data Type | Pre-aggregated dataset |
| Structure | Organized for analysis and visualization |
| Purpose | Dashboarding and insights generation |
- --

## 📊 GitHub Project: Ecommerce Sales Data Analysis Dashboard (Power BI)

### 📌 Project Overview

This project involves analyzing eCommerce sales data using Power BI, leveraging measures and DAX calculations to derive meaningful insights through interactive dashboards and visualizations.

The dashboard provides a comprehensive view of key business metrics such as:

* Total Orders
* Total Sales
* Total Profit
* Total Revenue
* Total Discount
* Year-to-Date (YTD) performance

---

### 📊 Dashboard Features

#### 🔹 Key Visualizations

* **Clustered Bar Chart**
  → Total Orders by Category and Region

* **Donut Chart**
  → Profit distribution by Category

* **Stacked Area Chart**
  → Monthly trend of Total Sales and Profit

* **Tree Map**
  → Total Sales by City, Region, and Quantity

* **Line & Stacked Column Chart**
  → Revenue and Sales comparison by Month

* **Funnel Chart**
  → Total Discount by Category

---

### 🎯 Interactive Capabilities

* Dynamic **filters and slicers**
* **Drill-down functionality** in Tree Map
* Clean and user-friendly layout
* Well-defined **titles, legends, and labels**

---

### 📤 Output

* Final dashboard exported as **PDF**
* Interactive `.pbix` file included for customization

---

## 📈 Summary Analysis

### 🔍 Key Insights

* **Sales & Revenue Trends**
  Monthly analysis shows fluctuations with peak sales periods indicating seasonal demand patterns.

* **Profitability by Category**
  Certain categories contribute significantly more profit, while others show lower margins despite high sales.

* **Regional Performance**
  Orders and sales vary across regions, highlighting top-performing markets and areas needing improvement.

* **Discount Impact**
  High discounts in some categories do not always translate into higher profits, indicating potential margin loss.

* **City-Level Contribution**
  Tree map reveals a few cities dominating total sales, suggesting strong localized demand.

---

### 💡 Business Recommendations

* Focus on **high-profit categories** for growth
* Optimize **discount strategies** to protect margins
* Strengthen marketing in **underperforming regions**
* Leverage **seasonal trends** for inventory planning

---

🚀 How to Use
Download the .pbix file
Open in Power BI Desktop
Explore dashboard using slicers and filters

<img width="669" height="504" alt="Ecommerce_Sales_Data_2024_2025" src="https://github.com/user-attachments/assets/8e657ead-37a4-48f4-9b6f-edfd6f138199" />

