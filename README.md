# 📊 Customer Shopping Behavior Analytics

**End-to-end retail analytics pipeline (Python, SQL, Power BI) to uncover customer behavior and drive data-driven decisions.**

---

## 📌 Overview

Retail businesses generate large volumes of transactional data but often lack clear insights into customer behavior. This project transforms raw shopping data into actionable intelligence by analyzing purchasing patterns, customer segments, and revenue drivers.

Using ~3,900 transactions, this project answers:
- What drives customer purchases?
- Which customers generate the most revenue?
- How behavior varies across demographics and channels?

**Target Users:**
- Data Analysts / Data Scientists  
- Business Intelligence Professionals  
- Recruiters evaluating analytics projects  

---

## 🚀 Key Features

- **Data Cleaning & Transformation (Python)**
  - Missing value imputation (category-based median)
  - Feature engineering (age groups, purchase frequency)
  - Column standardization

- **Relational Data Modeling (PostgreSQL)**
  - Structured schema for analytics
  - Efficient querying

- **SQL-Based Business Analysis**
  - Revenue segmentation (gender, age, subscription)
  - Customer segmentation (New, Returning, Loyal)
  - Product and discount analysis

- **Interactive Dashboard (Power BI)**
  - KPI tracking (revenue, avg spend, ratings)
  - Dynamic filtering

- **Business Insights**
  - Subscription vs non-subscription behavior
  - Discount-driven purchasing trends
  - High-value customer identification

---

## 🛠 Tech Stack

**Languages & Libraries**
- Python (Pandas, NumPy)

**Database**
- PostgreSQL

**Analytics**
- SQL (CTEs, aggregations, window functions)

**Visualization**
- Power BI

**Tools**
- Jupyter Notebook

---

## 🧠 Architecture / Workflow

```bash
Raw CSV Data
↓
Python (Cleaning & Feature Engineering)
↓
PostgreSQL (Storage)
↓
SQL (Analysis)
↓
Power BI (Visualization)
```

---

## ⚙️ Setup & Installation

### Prerequisites
- Python 3.8+
- PostgreSQL
- Power BI Desktop

---

### 1. Clone Repository
```bash
git clone https://github.com/your-username/customer-shopping-analytics.git
cd customer-shopping-analytics
```

### 2. Install Dependencies
```bash
pip install pandas numpy psycopg2
```

### 3. Run Data Pipeline
```bash
jupyter notebook
Open notebook
Run all cells to clean and load data
```

### 4. Setup Database
```bash
CREATE DATABASE retail_analytics;

Update DB credentials in the notebook before execution.
```
---

### 5. Open Dashboard

Open .pbix file in Power BI

📊 Usage

Example SQL Query

SELECT customer_segment, SUM(purchase_amount) AS total_revenue
FROM transactions
GROUP BY customer_segment
ORDER BY total_revenue DESC;

Workflow

Run Python notebook → prepare data

Load into PostgreSQL → structure data

Run SQL queries → generate insights

Open Power BI → visualize results

---

📈 Results / Impact

Majority customers are loyal buyers, driving most revenue

Young adults contribute the highest revenue share

Discount-heavy products influence purchasing decisions

Express shipping users spend more on average

Subscription users show comparable spending but lower total revenue

---

⚠️ Learnings / Challenges

Handling missing data using category-level imputation

Designing business-relevant features (not just technical ones)

Writing efficient SQL queries for large aggregations

Translating analysis into clear business insights

---


🤝 Contributing


Contributions are welcome.

Steps:

Fork the repo
Create a new branch
Submit a pull request
