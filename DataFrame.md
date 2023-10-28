# `DataFrame()`

- `DataFrame` is a 2D data structure that organizes data into `rows` and `columns`.
- It is like a spreadsheet, but with more features.
- `DataFrames` can be created from a variety of data sources, such as CSV files, Excel files, and SQL databases.

### `DataFrames` can be used to perform a variety of tasks, such as:

1. Cleaning and manipulating data
2. Analyzing data trends
3. Visualizing data using charts and graphs

### Benefits of using DataFrames:

1. `Flexibility`: DataFrames can be used to store a variety of data types, including numeric, categorical, and string data.
2. `Scalability`: DataFrames can scale to handle large datasets.
3. `Performance`: DataFrames are optimized for performance, so you can quickly and easily perform complex data operations.
4. `Ease of use`: DataFrames are easy to use, even for beginners.

### DataFrames can be created in multiple ways:

A. Using `List`
```python
import pandas as pd

# Create a list of lists:
list_of_lists = [['Kirankumar', 27, 'Mumbai'], ['Sumit', 26, 'Patna'], ['Suraj', 27, 'Bangalore']]

# Convert the list of lists to a DataFrame:
df = pd.DataFrame(list_of_lists, columns=['Name', 'Age', 'City'])

# Print the DataFrame:
print(df)
```

B. Using `zip`
```python
import pandas as pd

# Create lists of fields:
name = ['Kirankumar', 'Suraj', 'Sumit']
age = [27, 27, 26]
city = ['Mumbai', 'Bangalore', 'Patna']

# Combine the multiple lists into single list object:
df = pd.DataFrame(data=zip(name, age, city), columns=['Name', 'Age', 'City'])

# Print the DataFrame:
print(df)
```

C. Using `List` of `Dictionaries`
```python
import pandas as pd

# Create a list of dictionaries:
list_of_dictionaries = [{'Name': 'Kirankumar', 'Age': 27, 'Occupation': 'Data Scientist'}, {'Name': 'Suraj', 'Age': 27, 'Occupation': 'DevOps'}, {'Name': 'Sumit', 'Age': 26, 'Occupation': 'Python Developer'}]

# Convert the list of dictionaries to a DataFrame
df = pd.DataFrame(list_of_dictionaries)

# Print the DataFrame
print(df)
```
