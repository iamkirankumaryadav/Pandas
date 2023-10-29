# `Pandas` 🐼 Python Data Analysis Library 

Python library that help structure data in `DataFrames` and contain built-in functions for data analysis.

```python
import pandas as pd
```
### `Column` | `Feature` | `Attribute` | `Series` | `Field` | `Dimension`        

### `Row` | `Index` | `Record` | `Tuple` | `Observation` | `Sample`

- Pandas is an `exploratory data analysis toolkit` with rich set of [attributes](https://github.com/KIRANKUMAR7296/Pandas/blob/main/Attribute.md) and [methods](https://github.com/KIRANKUMAR7296/Pandas/blob/main/Method.md)
- Pandas provides a wide range of `functions` and `methods` 
- Widely used for `data cleaning`, `data exploration`, `data manipulation`, and `data analysis` tasks.
- `Toolkit` for reading, writing, [accessing](https://github.com/KIRANKUMAR7296/Pandas/blob/main/Access%20Data.md), filtering, [grouping](https://github.com/KIRANKUMAR7296/Pandas/blob/main/Grouping.md), aggregating, merging, joining, [combining](https://github.com/KIRANKUMAR7296/Pandas/blob/main/Combining.md), [reshaping](https://github.com/KIRANKUMAR7296/Pandas/blob/main/Reshaping.md), cleaning, selecting data and performing statistical computation.
- Financial term for `multidimensional structured data sets` is `Panel`
- Supports various formats of data: `csv`, `tsv`, `txt`, `xls`, `xlsx`, `json`, etc.
- `Performance optimization` ( Changing data types, storage type )
- Integrates well will other important libraries like `NumPy`, `Matplotlib`, `Seaborn`, `Scipy`, etc.

### Features of Pandas:

- Time series support
- Handling missing values
- Grouped operations
- Categorical data support
- Merging and joining DataFrames
- Statistical functions
- Data visualization tools

Data Type or Data Structure | Description
:--- | :--- 
`pandas.Series()` | `1D array` like object that can hold any data type.  
`pandas.DataFrame()` | `2D table` like data structure that can hold multiple types of data in columns.   

Attribute | Meaning
:--- | :---
`df.index` | Index labels of DataFrame ( Default: RangeIndex )
`df.columns` | Column labels of DataFrame  
`df.size` | Number of columns in DataFrame
`df.shape` | A tuple of rows and columns ( nrows, ncols )
`df.ndim` | Number of dimensions in the DataFrame ( 1D, 2D, 3D )
`df.values` | Values of DataFrame
`df.axes` | List containing index and columns

Method | Use
:--- | :---
`pd.read_csv()`, `pd.read_excel()`, `pd.read_json()` | Import data
`df.to_csv()`, `df.to_excel()`, `df.to_parquet()` | Export data
`df.head()`, `df.tail()`, `df.sample()`,`df.sort_values()` | Preview data
`df.query()` | Filter data
`df.iat[]`, `df.at[]`, `df.iloc[]`, `df.loc[]` | Indexing and Slicing
`df.info()` | Metadata Information
`df.dropna()`, `df.fillna()`, `df.drop_duplicates()`, `df.rename()`, `df.set_index()` | Clean data
`df.apply()`, `df.map()`, `df.reduce()`, `df.explode()` | Transform data
`df.groupby()`, `df.groupby().agg()`, `df.groupby().aggregate()` | Group and aggregate data
`df.join()`, `df.merge()`, `df.concat()` | Combine data
`df.pivot_table()`, `df.stack()`, `df.unstack()` | Reshape data 
`df.plot()` | Visualize data
`df.sum()`, `df.mean()`, `df.median()`, `df.max()`, `df.value_counts()`, `df.describe()` | Mathematical operations
`df.date_range()`, `df.to_datetime()` | Time Series analysis

### `Series` : 1D Array

- `Series` holds `homogeneous` data values, i.e. All data values are of `same` data type.
- Data axis labels are called as `index`

```python
# Create a series:
pd.Series([1, 2, 3, 4])

# Accessing a series:
DataFrame['SeriesName'] or DataFrame.SeriesName
```

<img src="Images/DataFrames.png" alt='DataFrame'>

### `DataFrame` : 2D Array

- Data is aligned in tabular form with `rows` and `columns`
- `DataFrame` is a sequence of `Series` that shares the same `index`

```python
# Empty DataFrame:
pd.DataFrame()

# Accessing DataFrame:
DataFrame[['SeriesName1', 'SeriesName2', 'SeriesName3']]
```

<img src="Images/PandasDataTypes.png" alt='DataFrame'>

<p align='right'><a align="right" href="https://github.com/KIRANKUMAR7296/Library/blob/main/Interview.md">Back to Questions</a></p>
