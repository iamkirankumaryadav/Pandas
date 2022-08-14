# `Access` Data

### `Index`

- Index object is an `immutable` array.
- There are two types of index in a DataFrame `row index` and `column index`
- Both indexes starts from `0`, allows to access a `row` or `column` using an index position or label name.

```python
# First row and first column:
df.iloc[0, 0]
```

# `Access` Data

`Method` | `Access` | Example
:--- | :--- | :---
`.at[]` | Access scalar value + Label based location | `df.at[1,'Country']` or `df['City'].at[1]`
`.iat[]` | Access scalar value + Integer based location | `df.iat[1,3]` or `df['City'].iat[1]`
`.loc[]` | Access record or field + Label based location | `df.loc[0,'City']` or `df['City'].loc[1]`
`.iloc[]` | Access record or field + Integer based location | `df.iloc[0,1]` or `df['City'].iloc[1]`

# Access `scalar` value 

### `DataFrame.at[]` : Label based location
```python
print(df.at[1, 'Country'])
```
### `DataFrame.iat[]` : Integer based location
```python
print(df.iat[1, 3])
```

# Access `scalar` value or entire `record` | `row` or `field` | `column`

### `DataFrame.loc[]` : Label based location
```python
# DataFrame.loc[]
print(df.loc[0, 'City'])

# Subset of DataFrame:
print(df.loc[[1, 2, 3], ['City', 'State', 'Country']])

# Slicing DataFrame:
print(df.loc[1:5, 'Name':'Country'])

# DataFrame.Series.loc[]
print(df['City'].loc[1])

# Subset of DataFrame:
print(df[['City', 'State', 'Country']].loc[[1, 2, 3]])

# Slicing DataFrame:
print(df['Name':'Country'].loc[1:5])
```      
### `DataFrame.iloc[]` : Integer based location
```python
# DataFrame.iloc[]
print(df.iloc[0, 1])

# Subset of DataFrame:
print(df.iloc[[1, 2, 3], [2, 4, 6]])

# Slicing DataFrame:
print(df.iloc[1:5, 1:6:2])

# DataFrame.Series.iloc[]
print(df['City'].iloc[1])

# Subset of DataFrame:
print(df[['City', 'State', 'Country']].iloc[[1, 2, 3]])

# Slicing DataFrame:
print(df['Name':'Country'].iloc[1:5])
```      
