# SQlite-sales-data-analysis
Files Included:
Jupyter notebook to analyze sales data from an SQLite database.
Bar chart showing revenue by pizza sizes.
SQLite database file containing the sales table.
Analyze sales data by querying the database, summarizing total quantity sold and revenue for each product, and visualizing it with a bar chart.
Connect to Database:
conn = sqlite3.connect("sales_data.db")
Run SQL Query
SELECT 
    product, 
    SUM(quantity) AS total_qty, 
    SUM(quantity * price) AS revenue
FROM sales
GROUP BY product
Load to Pandas
df = pd.read_sql_query(query, con
Display the result
print("Sales Summary by Product:")
print(df)
Print Output: Shows summarized data in tabular form.
Plot Revenue Bar Chart
![1000086800](https://github.com/user-attachments/assets/2ee09447-b684-4747-a9b1-d78054376e32)

