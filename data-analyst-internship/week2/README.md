# Week 2 – Python (Pandas) & SQL for Data Analysis

Welcome to **Week 2** of my data analytics portfolio (`rs-dot369/data-analytics-portfolio`). This week builds on Week 1 by moving into programmatic data manipulation with **Pandas** in Jupyter Notebook and structured querying with **SQL** on a 200-row sales dataset (`copy_SQL_Sales_Dataset_200_Rows.xlsx`).

---

## 📋 Overview & Tasks Completed

### Part 1: Python & Pandas Analysis (`week2_pandas_analysis.ipynb`)
1. **Data Loading & Inspection:** Loaded `copy_SQL_Sales_Dataset_200_Rows.xlsx` (200 rows, 10 columns: `order_id`, `customer_name`, `order_date`, `category`, `sub_category`, `product_name`, `quantity`, `unit_price`, `total_price`, `region`) and inspected `.head()`, `.info()`, and `.describe()`.
2. **Data Cleaning:** Checked for missing values and duplicate rows/order IDs (verified 0 missing values and 0 duplicates across all 200 records).
3. **Category Revenue Grouping:** Grouped sales data by `category` to compute total revenue, order count, and average order value.
4. **Multi-Column Sorting:** Sorted records across multiple fields—such as `region` (ascending) with `total_price` (descending), and `category` (ascending) with `order_date` (descending).
5. **Correlation Matrix:** Computed and visualized correlations across numerical columns (`quantity`, `unit_price`, `total_price`).

### Part 2: SQL for Data Analysis
* Practiced core SQL querying and aggregations (`SELECT`, `WHERE`, `GROUP BY`, `ORDER BY`, `SUM`, `AVG`, `COUNT`) to analyze top customers by spend and category-level revenue and average order values.
* Applied `CASE` statements to tier orders by value, subqueries to compare orders against overall average order value, and `JOIN`s to compare regional sales against target benchmarks.

---

## 📊 Key Results & Insights

* **Category Revenue Leaders:**
  * **Furniture:** `714,399` total revenue (`59` orders, avg order value `~12,108.46`)
  * **Grocery:** `672,147` total revenue (`49` orders, avg order value `~13,717.29`)
  * **Electronics:** `549,302` total revenue (`52` orders, avg order value `~10,563.50`)
  * **Clothing:** `484,259` total revenue (`40` orders, avg order value `~12,106.48`)
* **Correlation Findings (`quantity`, `unit_price`, `total_price`):**
  * `total_price` vs. `unit_price`: **`0.67`** (moderate-to-strong positive correlation)
  * `total_price` vs. `quantity`: **`0.66`** (strong positive correlation)
  * `quantity` vs. `unit_price`: **`0.05`** (negligible linear correlation—order quantities are fairly independent of unit price)
  * **Takeaway:** Both higher unit prices and larger order quantities contribute nearly equally to higher `total_price` values

---

## 🛠️ Tools & Technologies Used
* **Python:** `pandas`, `sqlite3`, `openpyxl`, `matplotlib`, `seaborn`
* **JupyterLab / Anaconda:** Interactive data exploration, analysis, and visualization
* **SQL:** Aggregations, filtering, sorting, `CASE` expressions, subqueries, and `JOIN`s
* **Git & GitHub:** Version control and portfolio documentation

---

## 📁 Folder Structure
```text
data-analytics-portfolio/
└── data-analyst-internship/
    ├── week1/
    └── week2/
        ├── copy_SQL_Sales_Dataset_200_Rows.xlsx
        ├── week2_pandas_analysis.ipynb
        ├── sql_queries_with_python.ipynb
        └── README.md
```        
