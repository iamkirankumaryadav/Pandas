# Pandas 🐼 

```python
import pandas as pd
```
### `Column` | `Feature` | `Attribute` | `Series` | `Field` | `Dimension`        

### `Row` | `Index` | `Record` | `Tuple` | `Observation` | `Sample`

- Pandas is an `exploratory data analysis toolkit` with rich set of <a href=><code>attributes</code></a> and `methods`
- `Toolkit` to `read`, `write`, `analyze`, `filter`, `manipulate`, `aggregate`, `merge`, `pivot` and `clean` the data.
- Financial term for a tabular data is `Panel`, supports various formats of data: `csv`, `tsv`, `txt`, `xls`, `xlsx`, `json`, etc.

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

- `Performance optimization` ( Changing data types, storage type )
- Integrates well will other important libraries like `NumPy`, `Matplotlib`, `Seaborn`
- Pandas is used in `economics`, `finance`, `statistics` and `analytics`

Data Types | Array
:--- | :---
`Series` | `1D`  
`DataFrame` | `2D`  
`Panel` | `3D` `major_axis` and `minor_axis` 
