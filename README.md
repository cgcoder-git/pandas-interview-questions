# pandas-interview-questions
top 30 pandas interview questions (instagram)

# Top-30-most-asked-Pandas-Questions-on-interview
here is the list contains the most asked questions in pandas

### 1. What is Pandas in Python, and why is it used?
Pandas is an open-source Python library for data manipulation and analysis, built on NumPy. It provides data structures like Series (1D) and DataFrame (2D) for handling structured data efficiently.
It’s used for data cleaning, transformation, aggregation, and visualization in data science and analytics.

### 2. What is the difference between a Pandas Series and a DataFrame?
A Series is a one-dimensional labeled array, while a DataFrame is a two-dimensional tabular structure with labeled rows and columns. A DataFrame can be thought of as a collection of Series.

![image](https://github.com/user-attachments/assets/e3457c93-aad4-4fd2-b9b4-f3f90e7fcf13)

### 3. Why doesn’t DataFrame.shape have parenthesis?
The reason DataFrame.shape in pandas doesn't have parentheses (i.e., it's used as df.shape instead of df.shape()) is because it's an attribute, not a method.
Attributes like shape, columns, and index are lightweight, always available, and do not change any data or perform calculations.

### 4. How do you add a new column to a Pandas DataFrame?
Assign values to a new column name using df['new_column_name'] = value 
or 
use assign().

![image](https://github.com/user-attachments/assets/1861df97-7e79-4715-8756-ad0fda9cd60a)

### 5. How do you remove columns from a Pandas DataFrame?
Use drop(columns=['col_name']) with axis=1
 or 
del df['col_name']

![image](https://github.com/user-attachments/assets/02ee166e-75d0-458b-bc23-eed116d76aad)

### 6. What is the difference between loc and iloc?
* You use .loc[] when you want to access rows or columns by their labels (i.e., the actual names like employee_id, emp_name etc)
* You Use .iloc[] when you want to access rows or columns by their numerical position (starting from 0).
  
![image](https://github.com/user-attachments/assets/5850fbfb-4544-4d3f-855c-d6674b6baa16)

### 7. How do you merge two DataFrames in Pandas?
In Pandas, you can merge two DataFrames using the merge() function, which is similar to SQL joins. It allows combining rows based on one or more keys (columns)

![image](https://github.com/user-attachments/assets/36e43f90-8c6f-447b-9b13-71a280e3fe1d)

### 8. What is the difference between the .join() and .merge() methods in pandas?
merge(): In Pandas, the merge() function is used to combine rows of two DataFrames based on one or more key columns, similar to SQL joins.
join():In Pandas, the join() method is used to combine two DataFrames on their index (by default), though you can join on a column as well. It’s more convenient for joining based on the index.

### 9. What is the purpose of the apply() function in Pandas?
apply() applies a function along an axis (rows/columns) or to a Series.

![image](https://github.com/user-attachments/assets/3a2ff697-6a3c-452b-bccf-db4c21be7abf)

### 10. How do you rename columns or indexes in a DataFrame?
Use rename() with columns or index parameters to rename labels.

![image](https://github.com/user-attachments/assets/d1cfe41c-8541-4cc5-a526-fa8244a755f9)

![image](https://github.com/user-attachments/assets/41e04508-b6a9-4279-a618-709b2e45e285)

### 11. Difference between fillna() and interpolate() methods
**fillna()**: Replaces missing values with a specified constant or method (like forward/backward fill).
**interpolate()**: estimates and fills missing values based on other data points using mathematical interpolation.
![image](https://github.com/user-attachments/assets/029db749-4b3c-4fd6-a0c3-1f2482014904)
Smoothly estimates missing values between 1 and 4 using linear interpolation.

### 12. What are common file formats Pandas can read from or write to?
list of common file formats that pandas can read from and write to:
                            Reading:
CSV: pd.**read_csv()**
Excel: pd.**read_excel()**
SQL: pd.**read_sql()**
JSON: pd.**read_json()**
                            Writing:
CSV: df.**to_csv()**
Excel: df.**to_excel()**

### 13. What is the astype() method, and why is it used?
**astype()**: astype is a method used to convert the DataType of a pandas Series or DataFrame column.
![image](https://github.com/user-attachments/assets/3fe7cac9-2496-4b3f-af68-099bb1b05e80)
Converting the grade column to category reduces memory usage, especially for columns with limited unique values.

### 14. How do you merge DataFrames with different key columns?
Using the **merge()** function with the left_on and right_on parameters you can merge columns with different names but representing the same data.
![image](https://github.com/user-attachments/assets/3b66544b-eebe-40fd-b3db-08148a0274be)

### 15: How do you check the memory usage of a DataFrame?
The primary method to check memory usage is DataFrame.**memory_usage()**, which provides the memory consumption of each column in bytes.

![image](https://github.com/user-attachments/assets/45d5acaa-3a7e-498c-8828-5ebcac570851)

### 16. What is the difference between groupby() and pivot_table()?
**groupby()**: Groups data and applies aggregate functions (e.g., sum, mean).
**pivot_table()**: More flexible than groupby, allows multi-level aggregation and reshaping similar to Excel pivot tables.
![image](https://github.com/user-attachments/assets/acc7a8a8-ee58-4e09-a092-a9726dd22f82)

### 17. What are common file formats Pandas can read from or write to?
Pandas offers several methods to handle missing data:
**dropna()**: Removes rows/columns with missing values.
**fillna()**: Fills missing values with a specified value or method (e.g., forward fill).
**interpolate()**: Fills missing values using interpolation techniques (linear, polynomial, etc.).

### 18. What is the difference between sort_values() and sort_index()?
**sort_values(by='column')**: Sorts by the values in one or more columns.
**sort_index()**: Sorts the DataFrame by its index (row labels).
![image](https://github.com/user-attachments/assets/8523002f-e5da-457b-8374-d7ec5d00bccd)

### 19. What is the difference between isin() and str.contains() in Pandas?
**isin()**: Used to filter rows where a column’s value is in a list of values.
**str.contains()**: Used with string columns to filter rows containing a specific substring.
![image](https://github.com/user-attachments/assets/765bb9ff-9265-48a1-a7b1-ef214e58be94)

### 20. How can you identify and handle outliers in a DataFrame?
Use statistical methods like IQR (Interquartile Range) or z-score.
![image](https://github.com/user-attachments/assets/5618bdbf-d558-4b73-af2a-f1450b147d84)
The interquartile range (IQR) formula is calculated as the difference between the third quartile (Q3) and the first quartile (Q1). In other words, IQR = Q3 - Q1.















