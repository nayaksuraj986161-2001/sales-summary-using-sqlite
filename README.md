# Basic Sales Summary from a Tiny SQLite Database using Python

## Project Overview

This project demonstrates how to use **SQLite inside Python** to store sales data, execute SQL queries, and generate basic sales summaries. The sales data is imported from a CSV file into a SQLite database, queried using SQL, and visualized with a simple bar chart using Matplotlib.

The objective of this project is to understand how SQL and Python work together for basic data analysis and reporting.

---

## Objective

* Create a SQLite database from a CSV dataset.
* Store sales records in a database table.
* Execute SQL queries inside Python.
* Generate a basic sales summary.
* Visualize sales revenue using a bar chart.

---

## Tools and Technologies

* Python 3
* SQLite3
* Pandas
* Matplotlib
* Jupyter Notebook
* Visual Studio Code

---

## Dataset

**Dataset Used:** Online Sales Data

The dataset contains product-level sales information including:

* Product Name
* Units Sold
* Total Revenue

Only the required columns were used for this project.

---

## Project Workflow

### Step 1: Import Required Libraries

* sqlite3
* pandas
* matplotlib.pyplot

### Step 2: Load Dataset

* Read the CSV file using Pandas.

### Step 3: Select Required Columns

Selected:

* Product Name
* Units Sold
* Total Revenue

### Step 4: Rename Columns

Renamed the columns as:

* product
* quantity
* revenue

### Step 5: Create SQLite Database

Created a database named:

```
sales_data.db
```

### Step 6: Store Data

Imported the cleaned data into the SQLite database as a table named:

```
sales
```

### Step 7: Execute SQL Query

Calculated:

* Total Quantity Sold
* Total Revenue

using SQL's `GROUP BY` statement.

### Step 8: Display Results

Displayed the SQL query output using Pandas.

### Step 9: Create Visualization

Generated a bar chart showing the **Top 10 Products by Revenue** using Matplotlib.

### Step 10: Save the Chart

Saved the visualization as:

```
sales_chart.png
```

---

## SQL Query Used

```sql
SELECT
    product,
    SUM(quantity) AS total_quantity,
    SUM(revenue) AS total_revenue
FROM sales
GROUP BY product;
```

---

## Project Structure

```
Task-7-Sales-Summary-SQLite/
│
├── Online Sales Data.csv
├── task7_sales_summary.ipynb
├── sales_data.db
├── sales_chart.png
└── README.md
```

---

## Output

The project successfully:

* Imported sales data into SQLite.
* Executed SQL queries inside Python.
* Generated a sales summary.
* Displayed query results.
* Created a revenue bar chart.
* Saved the visualization as an image.

---

## Learning Outcomes

After completing this project, I learned how to:

* Use SQLite with Python.
* Create a SQLite database programmatically.
* Store CSV data into a database.
* Execute SQL queries using Python.
* Retrieve SQL query results with Pandas.
* Perform basic sales analysis.
* Visualize results using Matplotlib.

---

## Future Improvements

* Add multiple SQL queries for deeper analysis.
* Create interactive visualizations.
* Build a dashboard using Power BI or Streamlit.
* Perform advanced sales analytics.

---

