# Statistics-and-ML
Detailed description of Advanced Analytics using Statistics and Practical Machine Learning in CDAC Mumbai.

## Course Overview
This repository contains a comprehensive 5-day training program covering fundamental concepts in Statistics, NumPy, Pandas, and Machine Learning. Each day builds upon the previous one to develop practical skills in data analysis and manipulation.

---

## Day 1: NumPy Fundamentals

**Reference:** [Day1.ipynb](Day1.ipynb)

Day 1 covers the foundational concepts of NumPy, the core library for numerical computing in Python. The session focuses on:

- **Array Creation & Manipulation**: Introduction to NumPy arrays and how they differ from Python lists
- **Array Generation Methods**: 
  - `np.arange()` - Creating arrays with specified start, stop, and step values
  - `np.linspace()` - Creating arrays with evenly spaced values over a specified interval
  - `np.append()`, `np.insert()`, `np.delete()` - Adding and removing elements from arrays
  - `np.concatenate()` - Combining multiple arrays

- **Array Reshaping**: Using `reshape()` to reorganize arrays into different dimensions (1D to 2D, 3D arrays, etc.)
- **Multi-dimensional Arrays**: Working with 2D and 3D arrays for matrix operations
- **Interview Preparation**: Discussion on common interview questions in data science, including performance and edge case considerations

---

## Day 2: NumPy Operations & Introduction to Pandas

**Reference:** [Day2.ipynb](Day2.ipynb)

Day 2 extends NumPy knowledge and introduces Pandas for data manipulation. Topics covered include:

- **Set Operations**:
  - `np.intersect1d()` - Finding common elements between arrays
  - `np.union1d()` - Combining unique elements from multiple arrays
  - `np.setdiff1d()` - Finding elements in one array but not in another
  - `np.setxor1d()` - Finding elements in either array but not in both
  - `np.isin()` - Checking membership of elements

- **Linear Algebra & Matrix Operations**:
  - Dot product and its geometric interpretation
  - Determinant calculation using `np.linalg.det()`
  - Cross product using `np.cross()`
  - Conditions for matrix multiplication

- **Random Number Generation**: Using `np.random.rand()` and `np.random.randint()` for generating random data

- **Introduction to Pandas**:
  - Creating Series objects with custom indices
  - Indexing methods: `iloc()` (position-based) vs `loc()` (label-based)
  - Concatenating Series using `pd.concat()`

---

## Day 3: Pandas - Data Loading & Exploration

**Reference:** [Day3.ipynb](Day3.ipynb)

Day 3 introduces practical data manipulation using Pandas with real-world datasets:

- **Data Loading**: Reading Excel files using `pd.read_excel()` with specific sheet names
- **Data Exploration**:
  - `head()` and `tail()` - Viewing first and last rows
  - `shape` - Understanding dataset dimensions
  - `unique()` - Finding distinct values in columns

- **Data Inspection**: Counting unique Material IDs and Locations in the CDAC dataset
- **Column Operations**: Renaming columns and accessing column values
- **Data Filtering**: Using `np.where()` to filter rows based on conditions (e.g., Quantity > 70)
- **Practical Application**: Analyzing ERP (Enterprise Resource Planning) data from the CDAC_DataBook.xlsx file

---

## Day 4: Pandas - Grouping, Aggregation & Visualization

**Reference:** [Day4.ipynb](Day4.ipynb)

Day 4 focuses on data aggregation and visualization techniques essential for data analysis:

- **GroupBy Operations**:
  - Single-column grouping using `groupby('MaterialID')`
  - Multi-column grouping using `groupby(['Location', 'MaterialID'])`
  - Accessing groups with `groups` attribute and `get_group()` method

- **Aggregation Functions**:
  - `agg('sum')` - Summing values by group
  - `agg(['sum', 'mean', 'size'])` - Multiple aggregations in one operation
  - Computing statistics like sum, mean, and count for grouped data

- **Sorting DataFrames**:
  - `sort_values()` - Sorting by column values
  - Ascending and descending order options
  - Preparing data for visualization

- **Data Visualization**:
  - Creating bar plots using Matplotlib and Seaborn
  - Visualization of top quantities by Material ID and Location
  - Customizing plot labels, titles, and formatting

---

## Day 5: Advanced Grouping & Data Reshaping

**Reference:** [Day5.ipynb](Day5.ipynb)

Day 5 covers advanced data manipulation and reshaping techniques:

- **GroupBy Operations Review**:
  - Reviewing single and multiple groupby operations
  - Computing mean, sum, and size statistics on grouped data
  - Accessing specific aggregated values using both label-based (`loc`) and position-based (`iloc`) indexing

- **Data Type Conversions**: Converting Series results to DataFrames for easier manipulation
- **Accessing Aggregated Results**: Multiple methods to retrieve specific values from aggregated data

- **Data Reshaping**:
  - **Long Format Conversion**: Using `melt()` to transform wide-format data into long format
  - Understanding the difference between wide and long data formats
  - Practical application on Health dataset from CDAC_DataBook.xlsx
  - Parameters: `id_vars` (columns to keep as identifiers), `var_name` (new column name for variables), `value_name` (new column name for values)

---

## Key Learning Outcomes

Upon completion of this 5-day course, participants will be able to:

1. Create, manipulate, and reshape NumPy arrays efficiently
2. Perform mathematical operations including linear algebra and matrix operations
3. Load and explore real-world datasets using Pandas
4. Filter and transform data based on specific conditions
5. Group data and compute aggregate statistics
6. Reshape data from wide to long formats
7. Create visualizations for exploratory data analysis
8. Prepare data for machine learning applications

---

## Tools & Libraries Used

- **NumPy**: Numerical computing and array operations
- **Pandas**: Data manipulation and analysis
- **Matplotlib**: Data visualization
- **Seaborn**: Statistical data visualization
- **Excel/XLS**: Data source format

---

## Dataset Reference

The practical examples throughout the course use the CDAC_DataBook.xlsx file containing:
- **ERPData sheet**: Enterprise Resource Planning data with MaterialID, Location, and Quantity information
- **Health sheet**: Health-related data for demonstrating data reshaping techniques
