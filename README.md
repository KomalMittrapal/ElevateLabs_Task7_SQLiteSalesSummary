# ElevateLabs_Task7_SQLiteSalesSummary
Get Basic Sales Summary from a Tiny SQLite Database using Python

# 🧮 Task 7: Basic Sales Summary using SQLite & Python

**Objective:** Use SQL inside Python to calculate total quantity and total revenue from a small sales database.

## 📂 Dataset
`retail_sales_dataset.csv` – Retail sales data used to create the SQLite database.

## 🧰 Tools Used

* Python
* SQLite3
* Pandas
* Matplotlib

## ⚙️ Prerequisites
Before running the code, ensure you have the following installed:

* **Python 3.8+**
* **Libraries:**  
  ```bash
  pip install pandas matplotlib
  ```

## 🧠 Steps Performed
1. Loaded the dataset (retail_sales_dataset.csv) into a Pandas DataFrame
2. Created a new SQLite database file — sales_data.db.
3. Inserted the DataFrame as a table named sales.
4. Wrote and executed SQL queries to calculate:
* Total quantity sold per product.
* Total revenue per product (SUM("Total Amount")).
5. Displayed query output using Pandas.
6. Visualized total revenue per product with a Matplotlib bar chart.
7. Saved the resulting chart as sales_chart.png.

## 🧾 Sample SQL Query
```sql
SELECT Produc Category, 
       SUM(Quantity) AS total_quantity_sold, 
       SUM("Total Amount") AS total_revenue
FROM sales
GROUP BY "Product Category";
```

## ✨ Analysis Results
- Printed a summary DataFrame showing each product’s total quantity sold and total revenue.
- Generated a bar chart comparing products by revenue.
- Identified top-selling and most profitable products at a glance.
### Output:

| Product | Total_Quantity | Total_Revenue |
|------------|-------------|-------------|
| Electronics | 849 | 156905 |
| Clothing | 894 | 155580 |
| Beauty | 771 | 143515 |

## 🖼 Visualization

A bar chart titled “Total Revenue by Product” was plotted and saved as sales_chart.png.

## 📂 Files in Repository
| File Name | Description |
|------------|-------------|
| `retail_sales_dataset.csv` | Original dataset |
| `task7_sales_summary.ipynb` | Python script performing SQL queries & visualization |
| `sales_data.db` | SQLite database generated |
| `sales_chart.png` | Output bar chart image |
| `README.md` | Project documentation file |

## 📊 Output

1. Printed summary table

2. Displayed bar chart of revenue by product

3. Saved chart as sales_chart.png

---
*Created by Komal for the Data Analyst Internship Program.*

