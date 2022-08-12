# Pandas 🐼 

```python
import pandas as pd
```
### `Column` | `Feature` | `Attribute` | `Series` | `Field` | `Dimension`        

### `Row` | `Index` | `Record` | `Tuple` | `Observation` | `Sample`

- `Toolkit` to `read`, `write`, `analyze`, `filter`, `manipulate`, `aggregate`, `merge`, `pivot` and `clean` the data.
- Financial term for a tabular data is `Panel`
- Pandas is an exploratory data analysis toolkit with rich set of `attributes` and `methods`
- Supports various formats of data: `csv`, `tsv`, `txt`, `xls`, `xlsx`, `json`, etc.

### `Attributes` 

Attribute | Meaning
:--- | :---
`df.index` | Index of DataFrame ( Default: RangeIndex )
`df.columns` | Columns in the DataFrame  
`df.size` | Number of fields in the DataFrame
`df.shape` | A tuple of number of rows and columns
`df.ndim` | Number of dimensions in the DataFrame (1D, 2D, 3D...)
`df.values` | All the values of the DataFrame
`df.axes` | List containing index and columns

### `Methods`

- `Import` data: `read_csv()`, `read_excel()`, `read_json()`
- `Export` data: `to_csv()`, `.to_excel()`
- `Preview` data: `head()`, `tail()`, `sample()`,`sort_values()`
- `Filter`, `Indexing` and `Slicing` data: `query()`, `loc[]`, `iloc`, `at[]`, `iat[]`       
- `Metadata`: `info()`
- `Clean` data: `dropna()`, `fillna()`, `drop_duplicates()`, `rename()`, `set_index()`
- `Transform` data: `apply()`, `map()`, `reduce()`, `explode()`
- `Group`, `Aggregate` and `Combine` data: `groupby()`, `join()`, `merge()`, `concat()`, 
- `Reshape` data: `pivot_table()`, `stack()` and `unstack()`
- `Visualize` data: `.plot()`
- `Mathematical` operations: `sum()`, `mean()`, `median()`, `max()`, `min()`, `value_counts()`, `describe()`
- `Time Series` Analysis: `date_range()`, `to_datetime()`
- `Performance optimization` ( Changing data types, storage type )
- Integrates well will other important libraries like `NumPy`, `Matplotlib`, `Seaborn`
- Pandas is used in `economics`, `finance`, `statistics` and `analytics`

### `Data Types`  

- `Series` ( `1D` array ), `DataFrames` ( `2D` array ) and `Panel` ( `3D` `major_axis` and `minor_axis` )  
