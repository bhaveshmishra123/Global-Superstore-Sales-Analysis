# 📊 Global Superstore Sales Analysis

## 📌 Project Overview

This project performs a **complete end-to-end data analysis** of the *Global Superstore Sales dataset*. The goal is to uncover meaningful business insights related to **sales performance, profitability, customer behavior, and logistics efficiency**.

The project demonstrates a full **data analytics workflow**, including:

* Data Loading
* Data Understanding
* Data Cleaning
* Exploratory Data Analysis (EDA)
* Feature Engineering
* Data Visualization
* Business Insights

The analysis was conducted using **Python**, followed by **SQL analysis** and **Power BI dashboards** to present business insights in an interactive format.

---

# 🛠️ Tech Stack

### Programming & Analysis

* Python
* Pandas
* NumPy
* SciPy
* Statsmodels

### Visualization

* Matplotlib
* Seaborn
* Plotly

### Data Tools

* SQL
* Power BI
* Excel (openpyxl)

---

# 📂 Dataset Information

The dataset contains **Global Superstore sales transactions** including customer information, product details, shipping data, and financial metrics.

### Dataset Size

* **Rows:** 51,290
* **Columns:** 24

### Key Data Categories

**Order Information**

* Order ID
* Order Date
* Ship Date
* Ship Mode
* Order Priority

**Customer Information**

* Customer ID
* Customer Name
* Segment

**Geographical Data**

* City
* State
* Country
* Region
* Market

**Product Details**

* Product ID
* Category
* Sub-Category
* Product Name

**Sales Metrics**

* Sales
* Quantity
* Discount
* Profit
* Shipping Cost

---

# 🔎 Data Analysis Workflow

## 1️⃣ Data Loading

The dataset is loaded using **Pandas** with `latin1` encoding to handle special characters.

```python
df = pd.read_csv('Global_Superstore2.csv', encoding='latin1')
```

---

# 📊 Data Understanding

Initial exploration was performed to understand dataset structure.

### Key Findings

* Dataset contains **51,290 records**
* **No duplicate rows**
* `Postal Code` has **~80% missing values**
* Date columns stored as **strings**
* Numerical metrics include sales, profit, quantity, discount, and shipping cost

---

# 🧹 Data Cleaning

Data preprocessing steps included:

### Handling Missing Values

* Missing values in **Postal Code** replaced with `0`

### Data Type Conversion

* Converted categorical columns to **category type**
* Converted **Order Date** and **Ship Date** to `datetime`

### Memory Optimization

Categorical conversion significantly reduced memory usage.

---

# 📈 Exploratory Data Analysis (EDA)

EDA was performed through **univariate, bivariate, and multivariate analysis**.

## Univariate Analysis

Analyzed distributions of individual variables such as:

* Sales
* Profit
* Discount
* Quantity
* Shipping Cost

Key observations:

* Sales distribution is **right-skewed**
* Profit contains **negative values indicating losses**

---

## Bivariate Analysis

Relationships between variables were analyzed.

### Key Relationships

**Sales vs Profit**

* Moderate positive correlation

**Discount vs Profit**

* Negative correlation

**Sales vs Shipping Cost**

* Strong positive correlation

These insights indicate that **high discounts significantly reduce profitability**.

---

## Multivariate Analysis

Advanced relationships were analyzed using **pivot tables and grouped statistics**.

Examples:

* Ship Mode vs Category vs Sales
* Segment vs Region vs Profit
* Region vs Ship Mode vs Sales & Profit

These analyses help identify **profitable segments and operational patterns**.

---

# ⚙️ Feature Engineering

Several new features were created to improve analytical insights.

### Profitability Features

* **Profit Margin**
* **Total Cost**
* **Loss Indicator**

### Time Features

* Order Year
* Order Month
* Order Quarter
* Order Delay

### Customer Behavior Features

* Customer Order Count
* Average Order Value

### Business Segmentation Features

* Revenue Category (Low / Medium / High)
* Shipping Speed (Fast / Medium / Slow)
* Discount Level

### Regional Metrics

* Region Profitability
* Market Profitability

These features allow deeper insights into **customer behavior, operational efficiency, and profitability patterns**.

---

# 📊 Data Visualization

Multiple visualizations were created to highlight important trends.

### Key Visualizations

* Pair Plot of Numeric Variables
* Sales Distribution Histogram
* Sales vs Profit Scatter Plot
* Total Sales by Category
* Orders by Customer Segment
* Region-wise Profitability
* Monthly Sales Trend
* Revenue Category Distribution
* Top Loss-Making Products

These charts help reveal **patterns, correlations, and outliers** within the dataset.

---

# 📈 Time Series Analysis

Monthly sales trends were analyzed to identify seasonal patterns.

### Key Findings

* Sales show **clear seasonal peaks**
* Strong growth trend over time
* Higher sales during **Q4 periods**

This insight can support **demand forecasting and inventory planning**.

---

# 🚚 Logistics Insights

Analysis of shipping modes revealed:

* **Standard Class generates the highest sales and profit**
* Faster shipping modes incur **higher operational costs**
* Shipping strategy directly impacts profitability

---

# 🌍 Regional Insights

Regional performance analysis shows:

* Some regions consistently generate **higher profits**
* Certain regions have **lower profitability or losses**
* Geographic analysis helps identify **growth opportunities**

---

# 📉 Loss Analysis

Loss-making products were identified through the **Loss feature**.

### Purpose

* Detect products generating consistent losses
* Support pricing and inventory decisions

This insight is crucial for **cost optimization and product strategy**.

---

# 📊 Power BI Dashboard

After completing the Python analysis, the dataset was exported and used to build **interactive Power BI dashboards**.

The dashboard includes:

* Sales Overview
* Profit Analysis
* Regional Performance
* Product Category Insights
* Customer Segmentation

Power BI enables **interactive business intelligence and executive reporting**.

---
# 🎥 Power BI Dashboard Demo

🎬 Watch the Power BI dashboard demonstration for this project:

👉 https://youtu.be/YOUR_VIDEO_LINK

In this demo, I showcase:

- Interactive Power BI dashboard
- Sales and profit analysis
- Region-wise performance insights
- Customer and product category analysis
- Key business insights derived from the dataset
---

# 🗄️ SQL Analysis

The cleaned dataset was also analyzed using **SQL** to perform:

* Aggregations
* Business KPI queries
* Regional and category comparisons
* Profitability analysis

SQL helps simulate **real-world data warehouse querying scenarios**.

---

# 💡 Key Business Insights

### 1. Sales & Growth

* Sales show steady long-term growth with seasonal spikes.

### 2. Discount Impact

* Higher discounts significantly reduce profit margins.

### 3. Customer Behavior

* Majority of customers fall into **moderate spending groups**.
* Small group of **high-value customers** drives significant revenue.

### 4. Product Performance

* Office Supplies contribute strong revenue.
* Some products generate consistent losses.

### 5. Shipping Strategy

* Standard shipping contributes most profit.
* Faster shipping options increase costs.

### 6. Regional Opportunities

* Certain regions have strong profitability potential.
* Others require cost optimization.

---

# 📁 Project Structure

```
Global-Superstore-Analysis
│
├── Data
│   └── Global_Superstore2.csv
│
├── Python Analysis
│   └── data_analysis.ipynb
│
├── SQL Analysis
│   └── sql_queries.sql
│
├── Power BI Dashboard
│   └── superstore_dashboard.pbix
│
├── Output Dataset
│   └── Output.csv
│
└── README.md
```

---

# 📌 Conclusion

This project demonstrates a **complete data analytics pipeline** combining:

* Python data analysis
* SQL querying
* Power BI visualization

The insights generated help businesses **optimize pricing strategies, improve logistics, and identify profitable markets and customers**.

---

# 👨‍💻 Author

**Bhavesh Kumar Mishra**
3rd Year Computer Science Engineering Student
Aspiring **Data Analyst**

---

⭐ If you found this project useful, consider giving it a **star on GitHub**!
