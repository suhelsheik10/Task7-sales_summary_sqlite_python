# Task 7 - Sales Summary using SQLite and Python

## 📊 Project Title: Basic Sales Summary using SQL in Python

This task was part of my Data Analyst internship, focusing on integrating SQL within Python to pull and visualize sales data from a SQLite database.

---

## 📂 Tools Used:
- **Python**
- **SQLite3**
- **Pandas**
- **Matplotlib**

---

## 📌 Objective:
To connect Python with a SQLite database, run SQL queries, summarize sales data (total quantity sold and total revenue), and visualize the results using a bar chart.

---

## 🧾 Dataset:
A small SQLite database `sales_data.db` was created manually using Python. It contains a single `sales` table with fields:
- `product`
- `quantity`
- `price`

---

## ✅ Steps Performed:
1. **Created a SQLite database and inserted sample sales data**
2. **Connected to the database using `sqlite3`**
3. **Ran an SQL query to group data by product and calculate total quantity and revenue**
4. **Loaded SQL output into a Pandas DataFrame**
5. **Printed the summary and plotted a bar chart using `matplotlib`**

---

## 🖥 Output:
- Printed Sales Summary (Total Quantity & Revenue)
- Bar Chart showing Revenue per Product
- Chart saved as `sales_chart.png`

---

## 📸 Screenshot
> Add screenshot of printed table and chart here (optional but recommended)

---

## 💬 Sample Interview Questions Answered:
- **How did you connect Python to a database?**  
  Using `sqlite3.connect("sales_data.db")`.

- **What SQL query did you run?**  
  `SELECT product, SUM(quantity), SUM(quantity * price) FROM sales GROUP BY product`.

- **What does GROUP BY do?**  
  It groups rows based on the product name, allowing aggregate functions like `SUM()`.

- **How did you calculate revenue?**  
  By using `SUM(quantity * price)` in SQL.

- **How did you visualize the result?**  
  Using `matplotlib` to create a bar chart of revenue vs product.

- **What does pandas do in your code?**  
  It reads SQL results into a DataFrame for easier manipulation and visualization.

- **What’s the benefit of using SQL inside Python?**  
  It combines data manipulation power of SQL with Python’s rich ecosystem for analysis and visualization.


