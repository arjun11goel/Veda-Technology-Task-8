# Task 8: Simple Data Filtering

## Objective
The objective of this task is to understand how conditional statements can be used to filter structured data in Python. We use a collection of student records (represented as a list of dictionaries) and apply various conditions to extract specific subsets of data.

## Execution Results

Here is the output from the data filtering operations:

```text
Original Student Records:
{'name': 'Alice', 'age': 20, 'department': 'Computer Science', 'marks': 85}
{'name': 'Bob', 'age': 22, 'department': 'Mechanical', 'marks': 72}
{'name': 'Charlie', 'age': 19, 'department': 'Computer Science', 'marks': 91}
{'name': 'David', 'age': 21, 'department': 'Electrical', 'marks': 65}
{'name': 'Eve', 'age': 20, 'department': 'Computer Science', 'marks': 78}

Students with marks greater than 80:
{'name': 'Alice', 'age': 20, 'department': 'Computer Science', 'marks': 85}
{'name': 'Charlie', 'age': 19, 'department': 'Computer Science', 'marks': 91}

Computer Science students aged 20:
{'name': 'Alice', 'age': 20, 'department': 'Computer Science', 'marks': 85}
{'name': 'Eve', 'age': 20, 'department': 'Computer Science', 'marks': 78}
```

## Interview Questions

**1. What is data filtering?**
Data filtering is the process of examining a dataset and extracting a specific subset of records that meet certain criteria or conditions. It allows you to ignore irrelevant data and focus only on the information necessary for your current analysis.

**2. How would you filter a Pandas DataFrame?**
You can filter a Pandas DataFrame using boolean indexing or the `.query()` method. 
*   **Boolean Indexing:** You create a condition that returns a boolean Series, and pass it to the DataFrame bracket notation. Example: `filtered_df = df[df['marks'] > 80]`
*   **Query Method:** You pass a condition as a string. Example: `filtered_df = df.query('marks > 80')`

**3. What is the difference between filtering and sorting?**
*   **Filtering** reduces the size of your dataset by hiding or removing records that do not match your specified conditions. It changes *what* data is visible.
*   **Sorting** simply changes the order of the records in the dataset (e.g., ascending or descending alphabetical or numerical order). It does not remove any records; it changes *how* the data is organized.
