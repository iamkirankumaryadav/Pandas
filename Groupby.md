# `Group By`

### `DataFrame.groupby()`

1. `Split` a DataFrame into groups based on filter.
2. Apply `aggregate` function on each group independently.
3. `Combine` each group into a DataFrame.

Returns a groupby object: `pandas.core.groupby.DataFrameGroupBy`

### `DataFrame.groupby()`

```python
# DataFrame.groupby(by='Column', axis=0, level=None, as_index=True, sort=True, group_keys=True, squeeze=False)
df.groupby(by=['City'])

# Iterating through groups:
for key, value in df.groupby(by=['City']):
      print(key)
      print(value)
      
# Group By Chaining: Date = 01/01/2022
df.groupby([df['Date'].str[:4], 'Product']).sum().reset_index().rename(columns={'Date': 'Year'}).head()
```                  
