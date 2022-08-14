# `Attribute`

<table>
  <tr>
    <th>Attribute</th> <th>Description</th>
  </tr>
  <tr><td><a href=#index><code>DataFrame.index</code></a></td> <td>Row labels of DataFrame</td></tr>
</table>

<h3 name=index>DataFrame.index</h3>

### `DataFrame.index` : Row labels of DataFrame.

```python
print(df.index)

# By default it automatically creates a RangeIndex(start=0, stop=len(df), step=1)
# We can manually add index by passing list to index parameter i.e. index = [1, 2, 3]
# We can also set some existing column as an index i.e index = 'City'
```

### `DataFrame.columns` : Columns labels of DataFrame.

```python
print(df.columns)
```

### `DataFrame.axes` : Label values of rows and columns in the DataFrame.

```python
print(df.axes)
```

### `DataFrame.dtypes` : Data types for each column of DataFrame.

```python
print(df.dtypes)
```

### `DataFrame.size` : Total number of elements in a DataFrame.

```python
print(df.size)
```

### `DataFrame.shape` : Dimensions of DataFrame ( Number of rows, Number of columns )

```python
# Dimensions of the dataframe:
print(df.shape)

# Extract only the total number of rows in a dataframe:
print(df.shape[0])

# Extract only the total number of columns in a dataframe:
print(df.shape[1])
```            

### `DataFrame.ndim` : Dimensions of DataFrame.

```python
print(df.ndim)
```

### `DataFrame.empty` : Check whether DataFrame is empty or not.

```python
print(df.empty)
```

### `DataFrame.T` : Change the rows into columns and columns into rows.

```python
print(df.T)
```

### `DataFrame.values` : Values of DataFrame in the form of NumPy array.

```python
print(df.values)
```
