# `Pandas` 🐼 Python Data Analysis Library 

```python
import pandas as pd
```
### `Column` | `Feature` | `Attribute` | `Series` | `Field` | `Dimension`        

### `Row` | `Index` | `Record` | `Tuple` | `Observation` | `Sample`

- Pandas is an `exploratory data analysis toolkit` with rich set of [attributes](https://github.com/KIRANKUMAR7296/Pandas/blob/main/Attribute.md) and [methods](https://github.com/KIRANKUMAR7296/Pandas/blob/main/Method.md)
- `Toolkit` for reading, writing, [accessing](https://github.com/KIRANKUMAR7296/Pandas/blob/main/Access%20Data.md), filtering, [grouping](https://github.com/KIRANKUMAR7296/Pandas/blob/main/Grouping.md), [combining](https://github.com/KIRANKUMAR7296/Pandas/blob/main/Combining.md), [reshaping](https://github.com/KIRANKUMAR7296/Pandas/blob/main/Reshaping.md) and cleaning data.
- Financial term for `multidimensional structured data sets` is `Panel`, supports various formats of data: `csv`, `tsv`, `txt`, `xls`, `xlsx`, `json`, etc.
- `Performance optimization` ( Changing data types, storage type )
- Integrates well will other important libraries like `NumPy`, `Matplotlib`, `Seaborn`
- Pandas is used in `economics`, `finance`, `statistics` and `analytics`

Data Types | Array
:--- | :---
`pandas.Series()` | `1D`  
`pandas.DataFrame()` | `2D`  

Attribute | Meaning
:--- | :---
`df.index` | Index of DataFrame ( Default: RangeIndex )
`df.columns` | Columns in the DataFrame  
`df.size` | Number of fields in the DataFrame
`df.shape` | A tuple of number of rows and columns
`df.ndim` | Number of dimensions in the DataFrame (1D, 2D, 3D...)
`df.values` | All the values of the DataFrame
`df.axes` | List containing index and columns

Method | Use
:--- | :---
`pd.read_csv()`, `pd.read_excel()`, `pd.read_json()` | Import data
`df.to_csv()`, `df.to_excel()` | Export data
`df.head()`, `df.tail()`, `df.sample()`,`df.sort_values()` | Preview data
`df.query()` | Filter data
`df.iat[]`, `df.at[]`, `df.iloc[]`, `df.loc[]` | Indexing and Slicing
`df.info()` | Metadata Information
`df.dropna()`, `df.fillna()`, `df.drop_duplicates()`, `df.rename()`, `df.set_index()` | Clean data
`df.apply()`, `df.map()`, `df.reduce()`, `df.explode()` | Transform data
`df.groupby()`, `df.join()`, `df.merge()`, `df.concat()` | Group by aggregate and combine data
`df.pivot_table()`, `df.stack()`, `df.unstack()` | Reshape data 
`df.plot()` | Visualize data
`df.sum()`, `df.mean()`, `df.median()`, `df.max()`, `df.value_counts()`, `df.describe()` | Mathematical operations
`df.date_range()`, `df.to_datetime()` | Time Series analysis
