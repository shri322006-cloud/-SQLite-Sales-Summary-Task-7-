# -SQLite-Sales-Summary-Task-7-
Task 7 - Basic Sales Summary using SQLite and Python (Data Analyst Internship). Includes SQLite database, SQL queries, Python script, and report with visualizations.
# SQLite Sales Summary (Task 7)

## 📌 Overview  
This repository contains the solution for **Task 7: Basic Sales Summary using SQLite and Python** as part of the **Data Analyst Internship**.  
The task demonstrates how to connect Python with SQLite, run SQL queries, and visualize the results using `matplotlib`.

---

## 📂 Contents  
- **sales_data.db** → SQLite database containing a small sales table.  
- **sales_task.py** → Python script to connect database, run SQL queries, and generate output.  
- **sales_summary_report.pdf** → Report with sales summary table and chart.  
- **sales_task_full_report.pdf** → Full report including SQL code, database info, query output, and chart.  
- **sales_chart.png** → Visualization of revenue by product.  

---

## ⚙️ Tools Used  
- Python (`sqlite3`, `pandas`, `matplotlib`)  
- SQLite (built-in with Python)  
- ReportLab (for PDF generation)  

---

## 📊 SQL Query Example  
```sql
SELECT product, 
       SUM(quantity) AS total_qty, 
       SUM(quantity * price) AS revenue
FROM sales
GROUP BY product;
