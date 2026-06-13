# Python-For-Data-Analysis-Internship
## NM - Oracle Arts Internship Program - Python Practice Projects

This repository tracks my daily progress, code snippets, and mini-projects during my internship. The progression moves from core Python fundamentals into procedural programming, and currently focuses on data manipulation and cleaning using industry-standard libraries like NumPy and Pandas.

## 🚀 Learning Log (Days 1 - 6)

### Day 1: Python Fundamentals & Control Flow
- **Environments:** Managed state and execution differences between local Jupyter Notebooks and Google Colab.
- **Core Concepts:** Variables, Collections (Lists, Tuples, Dictionaries, Sets), and conditional logic (`if-elif-else`, `for`, `while`).
- **Projects Built:** Student Marks Calculator, Expense Tracker, Grading System.
- **Debugging Victory:** Identified and solved the "hidden state" bug in Colab where counter variables must be explicitly re-initialized before loops.

### Day 2: Procedural Programming & File I/O
- **Modularity:** Built reusable functions for cleaner code execution.
- **Exception Handling:** Implemented robust `try-except-else-finally` blocks to gracefully handle invalid user inputs.
- **File Handling:** Read and wrote structured data using Python's `csv` module (`DictWriter` and `DictReader`).
- **Formatting:** Used f-string alignment operators (`<12`, `>5`) to generate clean console tables.

### Day 3: Introduction to NumPy & Vectorization
- **Transition:** Migrated from standard Python lists to `np.array` for high-performance mathematical operations.
- **Aggregations:** Replaced manual `for` loops with vectorized methods (`.sum()`, `.mean()`, `.max()`, `.min()`).
- **Projects Built:** Vectorized Student Scores Calculator and Monthly Sales Analyzer.

### Day 4: Advanced NumPy & Parallel Indexing
- **Data Mapping:** Implemented `np.argmax()` to map peak data points (highest sales) back to their corresponding categorical labels (product names).
- **Reporting:** Generated formatted product-wise sales units reports bridging arrays and lists.

### Day 5: Introduction to Pandas DataFrames
- **Structure:** Converted 1D arrays and Python dictionaries into 2D tabular `pd.DataFrame` structures.
- **Data Filtering:** Mastered Boolean Masking to filter datasets based on multiple conditions (e.g., department and experience level).
- **Categorical Analysis:** Utilized `.value_counts()` to instantly group and count occurrences.
- **Projects Built:** Employee Dataset Explorer.

### Day 6: Data Cleaning & Preprocessing Pipelines
- **Safe Loading:** Combined Day 2 exception handling with Pandas to safely load `messy_dataset.csv`.
- **Standardization:** Cleaned messy column headers using `df.rename()`.
- **Imputation:** Calculated column means to dynamically replace `NaN` values using `.fillna()` (refactored for Pandas 3.0 compliance without `inplace=True`).
- **Trimming:** Used `.dropna()` to remove incomplete records and `.drop_duplicates()` to clean repetitive entries.
- **Validation:** Verified pipeline success by checking the final `.shape` of the cleaned data.

---
*Author: Sugumaran J*
