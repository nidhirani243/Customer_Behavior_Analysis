# Customer_Behavior_Analysis
Data Analytics project showcasing customer behavior analysis using python, SQL and Power BI
# 📊 Data Analytics Project

## 📌 Overview

This project demonstrates an end-to-end **data analytics workflow** using Python, SQL, and Power BI.

The project focuses on transforming raw data into meaningful business insights through:

* Data loading and exploration using Python
* Exploratory Data Analysis (EDA)
* Data cleaning and preprocessing
* SQL analysis using PostgreSQL / MySQL / SQL Server
* Interactive dashboard development using Power BI
* Data-driven report preparation
* Presentation creation using Gamma

The goal is to analyze the dataset, identify important trends and patterns, and present actionable insights through visualizations and dashboards.

---

## 📂 Dataset

The project uses a structured dataset containing relevant business/analytical information.

### Dataset Workflow

1. Load the raw dataset using Python.
2. Understand the dataset structure and variables.
3. Check for:

   * Missing values
   * Duplicate records
   * Incorrect data types
   * Outliers
   * Inconsistent values
4. Clean and transform the data.
5. Use the cleaned dataset for SQL analysis and Power BI visualization.

**Dataset File:** `data/your_dataset.csv`

> Replace the dataset name and description with your actual dataset details.

---

## 🛠️ Tools & Technologies

| Tool                                | Purpose                                     |
| ----------------------------------- | ------------------------------------------- |
| **Python**                          | Data loading, cleaning and analysis         |
| **Pandas**                          | Data manipulation and preprocessing         |
| **NumPy**                           | Numerical analysis                          |
| **Matplotlib / Seaborn**            | Data visualization                          |
| **PostgreSQL / MySQL / SQL Server** | SQL-based data analysis                     |
| **Power BI**                        | Interactive dashboard and visualization     |
| **Gamma**                           | Project presentation                        |
| **Microsoft Excel**                 | Initial data inspection/supporting analysis |
| **Git & GitHub**                    | Version control and project documentation   |

---

## 🔄 Project Workflow

```text
Raw Dataset
     ↓
Data Loading using Python
     ↓
Exploratory Data Analysis (EDA)
     ↓
Data Cleaning & Preprocessing
     ↓
SQL Analysis
     ↓
Power BI Dashboard
     ↓
Business Insights & Results
     ↓
Report
     ↓
Gamma Presentation
```

---

## 🐍 Step 1: Data Loading

The dataset is imported into Python using Pandas.

```python
import pandas as pd

df = pd.read_csv("data/your_dataset.csv")

print(df.head())
print(df.info())
print(df.shape)
```

The initial analysis helps understand the dataset's structure, number of records, columns, and data types.

---

## 🔎 Step 2: Exploratory Data Analysis

EDA is performed to understand the characteristics and patterns within the dataset.

### Key Analysis

* Dataset dimensions
* Column data types
* Statistical summary
* Missing values
* Duplicate records
* Unique values
* Distribution of numerical variables
* Relationships between variables
* Trends and patterns

Example:

```python
df.describe()
df.isnull().sum()
df.duplicated().sum()
```

Visualizations are created to identify important patterns and relationships in the data.

---

## 🧹 Step 3: Data Cleaning

The raw dataset is cleaned before performing further analysis.

### Cleaning Tasks

* Handling missing values
* Removing duplicate records
* Correcting data types
* Standardizing categorical values
* Handling inconsistent records
* Identifying and treating outliers where required
* Creating useful calculated columns

The cleaned dataset is then exported for SQL analysis and Power BI.

```python
df.to_csv("data/cleaned_dataset.csv", index=False)
```

---

## 🗄️ Step 4: SQL Analysis

The cleaned dataset is imported into a relational database such as **PostgreSQL, MySQL, or SQL Server**.

SQL queries are used to answer important business questions.

### SQL Concepts Used

* `SELECT`
* `WHERE`
* `GROUP BY`
* `ORDER BY`
* Aggregate functions
* `CASE WHEN`
* `JOIN`
* Subqueries
* Common Table Expressions (CTEs)
* Window functions

Example:

```sql
SELECT category,
       COUNT(*) AS total_records,
       SUM(amount) AS total_amount
FROM sales
GROUP BY category
ORDER BY total_amount DESC;
```

The SQL analysis helps identify trends, top-performing categories, key metrics, and other business insights.

---

## 📊 Step 5: Power BI Dashboard

The cleaned data and SQL analysis are used to create an interactive **Power BI dashboard**.

### Dashboard Features

* KPI cards
* Interactive charts
* Trend analysis
* Category-wise analysis
* Filters and slicers
* Comparative analysis
* Geographic analysis (if applicable)
* Drill-down analysis where required

### Key KPIs

Examples include:

* Total Records
* Total Sales/Revenue
* Average Value
* Growth Rate
* Customer Count
* Top-performing Category

> Replace these KPIs with the actual KPIs used in your project.

### Dashboard Preview

Add your Power BI dashboard screenshot here:

```markdown
![Power BI Dashboard](images/dashboard.png)
```

---

## 📈 Results & Insights

The analysis provides meaningful insights from the dataset.

### Key Findings

* Identified major trends and patterns in the data.
* Determined top-performing categories/products/segments.
* Identified areas with low or high performance.
* Analyzed changes over time.
* Compared different business segments using SQL.
* Created an interactive dashboard for easier decision-making.

> Add 3–5 specific insights from your actual analysis here. Quantified insights are preferred.

Example:

* Category A generated the highest overall revenue.
* Region B recorded the highest number of transactions.
* Sales increased significantly during the final quarter.
* A small number of categories contributed a large percentage of total revenue.

---

## 📑 Project Report

A detailed report was prepared covering:

1. Project Introduction
2. Business Problem
3. Dataset Description
4. Data Cleaning
5. Exploratory Data Analysis
6. SQL Analysis
7. Power BI Dashboard
8. Key Insights
9. Recommendations
10. Conclusion

**Report:** `reports/project_report.pdf`

---

## 🎤 Project Presentation

A presentation was created using **Gamma** to communicate the project findings in a concise and professional format.

The presentation includes:

* Business Problem
* Dataset
* Methodology
* Data Analysis
* SQL Insights
* Power BI Dashboard
* Key Findings
* Recommendations
* Conclusion

**Presentation:** `presentation/project_presentation.pdf`

---

## 🚀 How to Run

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/your-repository-name.git
cd your-repository-name
```

### 2. Install Python Dependencies

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### 3. Open the Python Notebook

```bash
jupyter notebook
```

Open the notebook located in:

```text
notebooks/
```

### 4. Run the Analysis

Run the notebook cells sequentially to:

* Load the dataset
* Perform EDA
* Clean the data
* Generate visualizations
* Export the cleaned dataset

### 5. Run SQL Analysis

Import the cleaned dataset into your preferred database:

* PostgreSQL
* MySQL
* SQL Server

Then execute the SQL scripts available in:

```text
sql/
```

### 6. Open Power BI Dashboard

Open the Power BI file:

```text
powerbi/project_dashboard.pbix
```

If required, update the data source connection and refresh the dashboard.

---

## 📁 Project Structure

```text
Data-Analytics-Project/
│
├── data/
│   ├── raw_dataset.csv
│   └── cleaned_dataset.csv
│
├── notebooks/
│   └── data_analysis.ipynb
│
├── sql/
│   └── analysis_queries.sql
│
├── powerbi/
│   └── project_dashboard.pbix
│
├── reports/
│   └── project_report.pdf
│
├── presentation/
│   └── project_presentation.pdf
│
├── images/
│   └── dashboard.png
│
├── requirements.txt
└── README.md
```

---

## 💡 Skills Demonstrated

This project demonstrates practical experience in:

* Data Cleaning
* Exploratory Data Analysis
* Python for Data Analytics
* Pandas & NumPy
* SQL
* PostgreSQL / MySQL / SQL Server
* Data Visualization
* Power BI
* Dashboard Development
* Business Intelligence
* Data Storytelling
* Business Reporting
* Presentation Development

---

## 👤 Author

**Nidhi Rani**

B.Tech Computer Science Engineering | Aspiring Data Analyst

📍 Bhopal, India

---

## ⭐ Conclusion

This project demonstrates an end-to-end approach to solving a data analytics problem — from **raw data preparation and exploratory analysis to SQL querying, interactive Power BI visualization, and business reporting**.

The project highlights the ability to transform raw data into **clear, actionable insights that can support data-driven decision-making**.
