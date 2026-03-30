## Lab Report: Introduction to Pandas
**Student Name:** Vedant Trivedi  
**PRN:** 25070123121  
**Experiment No:** 10

### 1. Aim
To explore the core components of the `pandas` library, including Series and DataFrames, and to perform basic data manipulation tasks such as indexing, selection, updating, and filtering.

### 2. Theory
Pandas is built on two primary data structures:
* **Series:** A 1D array-like object that can hold any data type. Think of it as a single column in a spreadsheet.
* **DataFrame:** A 2D, size-mutable, tabular data structure with labeled axes (rows and columns).
* **Indexing & Selection:** * `.loc[]`: Label-based selection (uses column names and row index labels).
    * `.iloc[]`: Integer-based selection (uses numerical positions starting from 0).
* **Data Wrangling:** The ability to add new columns, drop unnecessary ones, and update specific values based on conditions.

### 3. Logic
The experiment follows a logical progression of data interaction:
1.  **Creation:** Initializing data structures from lists (Series) and dictionaries (DataFrame).
2.  **Metadata Inspection:** Understanding the dimensions and "shape" of the object.
3.  **Manipulation:** Changing data values and adding derived columns (like 'grade').
4.  **Transformation:** Removing columns (`drop`) and calculating summary statistics (`mean`, `min`, `max`).
5.  **Selection:** Filtering the dataset to extract only the information that meets specific criteria (Boolean indexing).

### 4. One-Liner Code Explanations
* `pd.Series([10, 20...])`: Creates a one-dimensional labeled array.
* `pd.DataFrame(data)`: Combines multiple Series-like structures into a two-dimensional table.
* `df.shape` / `df.ndim`: Returns the dimensions (rows/cols) and the number of axes (2 for a DataFrame).
* `df.dtypes`: Shows the data format (int, object, float) for every column.
* `df.loc[0, "Name"]`: Accesses a specific value using its row index and column label.
* `df.iloc[1, 1]`: Accesses a specific value using its exact integer coordinates.
* `df["grade"] = [...]`: Dynamically adds a new column to an existing DataFrame.
* `df.drop("grade", axis=1)`: Removes a specific column without deleting the row data.
* `df["MARKS"].mean()`: Calculates the arithmetic average of a specific column.
* `df[df["MARKS"] > 80]`: Filters the rows to show only students with marks exceeding 80.

### 5. Algorithm
1.  **Import** `pandas`.
2.  **Initialize** a Series to understand 1D data.
3.  **Construct** a DataFrame using a dictionary of lists.
4.  **Query** structural attributes like `shape`, `size`, and `columns`.
5.  **Access Data** using both label-based (`loc`) and position-based (`iloc`) indexing.
6.  **Modify** the DataFrame by adding a 'grade' column based on performance.
7.  **Update** existing values to reflect corrections (e.g., updating Student A's marks).
8.  **Delete** unwanted columns using the `drop` method.
9.  **Analyze** the data using statistical functions (`min`, `max`, `mean`).
10. **Filter** the results using a Boolean condition to isolate high-performers.

### 6. Conclusion
Experimenting with Pandas revealed how effortlessly structured data can be manipulated in Python compared to standard lists. I learned that `loc` and `iloc` are essential for precise data targeting and that DataFrames are highly flexible—allowing for real-time updates and filtering. This ability to clean and analyze data programmatically is a fundamental skill for any data analyst.

---
