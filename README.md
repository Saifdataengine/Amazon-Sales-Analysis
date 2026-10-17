# Amazon Sales Analysis 📊
### An Exploratory Data Analysis (EDA) and Business Intelligence Project

**Author:** Saif Ali Khan  
**Tools:** Python, Pandas, NumPy, Matplotlib, Seaborn, Power BI, Jupyter Notebook  
**Dataset:** Amazon Sale Report  
**Domain:** Data Analytics | EDA | Business Intelligence

---

## 📌 Table of Contents

- [Project Overview](#-project-overview)
- [Project Objectives](#-project-objectives)
- [Dataset Description](#-dataset-description)
- [Tools and Technologies](#-tools-and-technologies)
- [Project Workflow](#-project-workflow)
- [Key Performance Indicators](#-key-performance-indicators)
- [Exploratory Data Analysis](#-exploratory-data-analysis)
- [Key Business Insights](#-key-business-insights)
- [Power BI Dashboard](#-power-bi-dashboard)
- [Business Recommendations](#-business-recommendations)
- [Project Structure](#-project-structure)
- [Installation and Usage](#-installation-and-usage)
- [Limitations](#-limitations)
- [Conclusion](#-conclusion)

---

## 📌 Project Overview

The **Amazon Sales Analysis** project explores Amazon.in sales data to understand product demand, sales patterns, order fulfilment methods, shipping preferences, cancellations, and geographical distribution.

Python is used for data inspection, cleaning, exploratory data analysis (EDA), and visualization. Power BI is used to present key metrics and business findings through an interactive dashboard.

The primary objective is to transform raw sales data into meaningful insights that help identify operational challenges, understand product performance, and support data-driven business decisions.

## 🎯 Project Objectives

- Analyze overall order volume and sales performance.
- Identify high-demand product categories.
- Examine order statuses, cancellations, and returns.
- Compare Amazon and Merchant fulfilment methods.
- Analyze shipping service-level distributions.
- Explore sales and order trends over time.
- Identify missing values and data-quality issues.
- Understand geographical sales patterns across states and cities.
- Create meaningful data visualizations.
- Develop an interactive Power BI dashboard.
- Generate actionable business insights and recommendations.

## 📂 Dataset Description

The project uses the **Amazon Sale Report** dataset, containing order records, product information, fulfilment details, shipping information, and sales amounts.

| Dataset Attribute | Description |
|---|---|
| Dataset Name | Amazon Sale Report |
| File Format | CSV |
| Total Records | 128,975 |
| Total Columns | 24 |
| Currency | Indian Rupees (INR), where applicable |
| Data Period | April 2022 onward, based on the dataset's date field |

### Important Columns

| Column | Description |
|---|---|
| `Order ID` | Identifier associated with an order |
| `Date` | Order date |
| `Status` | Recorded order status |
| `Fulfilment` | Order fulfilment method |
| `Sales Channel ` | Channel through which the order was placed |
| `ship-service-level` | Shipping service level |
| `SKU` | Stock Keeping Unit identifier |
| `Category` | Product category |
| `Size` | Product size |
| `Qty` | Quantity associated with the record |
| `Amount` | Recorded order amount |
| `Courier Status` | Courier-related status |
| `ship-city` | Customer shipping city |
| `ship-state` | Customer shipping state |
| `ship-country` | Customer shipping country |
| `ship-postal-code` | Customer shipping postal code |
| `promotion-ids` | Associated promotional identifiers |
| `B2B` | Business-to-business order indicator |
| `fulfilled-by` | Fulfilment provider information |

Other columns, including `Style`, `ASIN`, `currency`, and `Unnamed: 22`, provide additional information for analysis and data-quality assessment.

## 🛠️ Tools and Technologies

| Tool | Purpose |
|---|---|
| Python | Data analysis and automation |
| Pandas | Data manipulation and cleaning |
| NumPy | Numerical operations |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization |
| Jupyter Notebook | Performing and documenting EDA |
| Power BI | Interactive dashboard development |

## 🔄 Project Workflow

### Step 1: Data Loading and Inspection
- Imported the CSV dataset into Python.
- Examined dataset dimensions and structure.
- Reviewed column names and data types.
- Identified potential data-quality issues.

### Step 2: Data Quality Assessment
- Checked missing values across columns.
- Examined exact duplicate records.
- Reviewed inconsistent values and data types.
- Investigated unnecessary or unexpected columns.

### Step 3: Data Cleaning
- Standardized column names where necessary.
- Corrected data types where appropriate.
- Investigated missing values before deciding how to handle them.
- Reviewed duplicate records without automatically removing potentially valid order-item records.
- Checked inconsistent and unexpected values.

### Step 4: Exploratory Data Analysis (EDA)
- Analyzed categorical variables.
- Examined numerical variables, including `Qty` and `Amount`.
- Investigated product-category distribution.
- Explored order statuses and fulfilment methods.
- Examined shipping service levels.
- Investigated relationships between relevant numerical variables.

### Step 5: Data Visualization
Created visualizations to understand patterns and communicate findings, including:
- Product-category comparisons.
- Quantity and sales amount distributions.
- Order-status distribution.
- Fulfilment and shipping comparisons.
- Time-based trends.
- Geographical order distribution.

### Step 6: Business Insights
- Identified high-volume product categories.
- Examined fulfilment and shipping distributions.
- Investigated order cancellations.
- Highlighted missing-value issues.
- Developed recommendations based on observed patterns.

### Step 7: Dashboard Development
Used Power BI to present important metrics and analytical findings through an interactive dashboard.

## 📈 Key Performance Indicators (KPIs)

The following metrics were identified from the uploaded raw dataset.

| Metric | Value |
|---|---:|
| Total Records | 128,975 |
| Total Columns | 24 |
| Available Amount Values — Sum | ₹78,592,678.30 |
| Records with Amount Values | 121,180 |
| Total Quantity | 116,649 |
| Cancelled Records | 18,332 |
| Cancellation Share of All Records | Approximately 14.21% |
| Amazon Fulfilment Share | Approximately 69.55% |
| Expedited Shipping Share | Approximately 68.71% |
| Missing Amount Values | 7,795 |

> **Important:** These figures represent the raw dataset. Metrics may change after cleaning, filtering, or applying business rules. The sum of available `Amount` values should not automatically be treated as realized revenue because it may include cancelled or other non-completed orders. The cancellation percentage shown above is based on records, not necessarily unique orders or a confirmed order-level cancellation rate.

## 🔍 Exploratory Data Analysis

### 1. Product Category Analysis
- Identify categories with the highest record counts.
- Compare category-wise quantities and sales amounts.
- Understand the distribution of recorded product activity.

### 2. Order Status Analysis
- Examine the distribution of order statuses.
- Investigate cancellations and returns.
- Identify categories or periods that may require further analysis.

### 3. Fulfilment Analysis
- Compare Amazon and Merchant fulfilment.
- Examine fulfilment distribution across recorded orders.
- Investigate differences in cancellation and courier statuses.

### 4. Shipping Analysis
- Compare Expedited and Standard shipping.
- Examine shipping service-level distribution.
- Investigate relationships between shipping methods and order outcomes.

### 5. Sales and Quantity Analysis
- Analyze the distribution of `Amount` and `Qty`.
- Identify unusual values and potential outliers.
- Compare category-wise sales amounts and quantities.

### 6. Time-Series Analysis
- Explore monthly and daily order patterns.
- Analyze changes in order volume over time.
- Investigate possible seasonal patterns.

### 7. Geographical Analysis
- Examine order distribution by state and city.
- Identify locations with high recorded order volumes.
- Explore geographical patterns to support inventory and delivery planning.

### 8. Data Quality Analysis
- Investigate missing values.
- Review unexpected columns and inconsistent data.
- Check exact duplicates and repeated order identifiers.
- Validate data before calculating final business KPIs.

## 💡 Key Business Insights

### 1. Product Category Performance
The `Set` and `kurta` categories have the highest record counts in the uploaded dataset.

**Business implication:** These categories represent a substantial share of recorded product activity and deserve further investigation.

**Recommendation:** Compare their sales contribution, quantity, and order outcomes before making inventory or promotional decisions.

### 2. Fulfilment Distribution
- Amazon Fulfilment: approximately 69.55%.
- Merchant Fulfilment: approximately 30.45%.

Amazon Fulfilment accounts for the larger share of recorded records.

**Recommendation:** Compare cancellation rates and available courier outcomes across fulfilment methods to identify possible operational differences.

### 3. Shipping Service Levels
Expedited shipping accounts for approximately 68.71% of records.

This indicates that Expedited shipping represents a substantial portion of the dataset. However, the distribution alone does not prove customer preference or better shipping performance.

**Recommendation:** Compare shipping methods using cancellation rates, recorded statuses, and available courier information.

### 4. Order Cancellation Analysis
The raw dataset contains 18,332 cancelled records, representing approximately 14.21% of all records.

**Recommendation:** Investigate cancellations by category, fulfilment method, shipping service level, and month. Validate the results using unique-order counts where appropriate.

### 5. Sales Amount Analysis
The sum of available `Amount` values is approximately ₹7.86 crore, while 7,795 records have missing amounts.

**Recommendation:** Investigate missing amounts and define rules for completed orders before reporting realized revenue.

### 6. Data Quality Issues
The dataset contains missing values in fields such as `Amount`, `promotion-ids`, `fulfilled-by`, and certain courier or shipping-location fields. An unexpected column named `Unnamed: 22` is also present.

The raw dataset had no exact full-row duplicates according to the initial check. Repeated `Order ID` values may still be legitimate because one order can contain multiple item-level records.

**Recommendation:** Document data-cleaning decisions and validate important fields before publishing final metrics.

## 📊 Power BI Dashboard

The Power BI dashboard is intended to communicate the project's findings through interactive visualizations.

### Planned Dashboard Components
- **KPI Cards:** Total records, total quantity, available sales amount, and cancellation metrics.
- **Category Analysis:** Product-category distribution and category-wise sales amounts.
- **Order Status Analysis:** Status distribution and cancelled records.
- **Fulfilment Analysis:** Amazon versus Merchant fulfilment.
- **Shipping Analysis:** Expedited versus Standard shipping.
- **Time-Series Analysis:** Order and sales trends by date or month.
- **Geographical Analysis:** State-wise and city-wise order distribution.
- **Numerical Analysis:** Relationships between quantity and sales amount.

Dashboard filters can help users explore the data by date, category, fulfilment method, shipping level, and geographical location.

Add a screenshot of the completed dashboard to the repository's `images/` folder and embed it here when available:

```markdown
![Amazon Sales Dashboard](images/dashboard.png)
```

## 🚀 Business Recommendations

1. **Improve inventory planning:** Monitor demand for high-volume product categories.
2. **Investigate cancellations:** Identify patterns across categories, fulfilment methods, and time periods.
3. **Evaluate fulfilment performance:** Compare Amazon and Merchant fulfilment using relevant operational indicators.
4. **Validate sales data:** Investigate missing `Amount` values before calculating revenue-related KPIs.
5. **Analyze shipping outcomes:** Compare shipping methods using recorded order and courier statuses.
6. **Explore geographical demand:** Use state-wise and city-wise order patterns to support inventory planning.
7. **Monitor sales trends:** Analyze monthly order activity to investigate possible seasonal variations.
8. **Improve data quality:** Document cleaning rules and validate the dataset before producing final reports.

These recommendations identify areas for further analysis. Their actual business impact should be evaluated using additional evidence.

## 📁 Project Structure

A suggested GitHub repository structure is shown below:

```text
Amazon-Sales-Analysis/
│
├── data/
│   └── README.md
│
├── notebooks/
│   └── amazon_sales_analysis.ipynb
│
├── images/
│   └── dashboard.png
│
├── reports/
│   └── Amazon_Sales_Analysis_Report.pdf
│
├── README.md
└── requirements.txt
```

**Note:** Include only files that actually exist in your project. If the original dataset cannot be redistributed, provide instructions for obtaining it rather than uploading the raw CSV.

## ⚙️ Installation and Usage

### Prerequisites
- Python 3
- Jupyter Notebook
- Power BI Desktop (for the dashboard)

### 1. Clone the Repository

```bash
git clone <your-github-repository-url>
cd Amazon-Sales-Analysis
```

Replace the placeholder with your actual GitHub repository URL.

### 2. Install Required Libraries

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### 3. Add the Dataset

Place the dataset in the appropriate directory and update the file path in the notebook.

Example:

```python
import pandas as pd

df = pd.read_csv("../data/Amazon Sale Report.csv")

print(df.head())
print(df.shape)
print(df.info())
```

Update the path according to your actual folder structure and filename.

### 4. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open `amazon_sales_analysis.ipynb` and execute the cells in order.

### 5. Open the Power BI Dashboard

If a `.pbix` file is included in the repository, open it using Power BI Desktop to explore the dashboard.

## ⚠️ Limitations

- Missing values may affect the completeness of certain analyses.
- The raw sum of `Amount` is not necessarily net realized revenue.
- Raw record counts and unique-order counts are different metrics.
- Cancellation percentages depend on the chosen denominator and business rules.
- Some findings require validation after data cleaning.
- The analysis identifies associations and patterns but does not establish causation.
- Recommendations should be validated before being used for major business decisions.

## 📝 Conclusion

The **Amazon Sales Analysis** project demonstrates how raw e-commerce sales data can be transformed into meaningful business insights using data cleaning, exploratory data analysis, and visualization.

The analysis explores product-category demand, fulfilment methods, shipping distributions, cancellation patterns, geographical activity, and data-quality issues.

The initial findings highlight opportunities to investigate cancellations, improve inventory planning, evaluate fulfilment performance, and strengthen sales reporting.

By combining Python-based analysis with Power BI visualization, the project provides a structured approach to understanding e-commerce data and supporting data-driven decision-making.

---

## 👨‍💻 Author

**Saif Ali Khan**

- **Project:** Amazon Sales Analysis
- **Focus:** Data Analytics and Business Intelligence
- **Technologies:** Python, Pandas, NumPy, Matplotlib, Seaborn, Power BI, Jupyter Notebook

This project demonstrates practical skills in data cleaning, exploratory data analysis, data visualization, and business insight generation.
