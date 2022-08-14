# `Attribute`

<table>
  <tr><th><h3>Attribute</h3></th> <th><h3>Description</h3></th></tr>
  <tr><td><a href=#index><code>DataFrame.index</code></a></td> <td>Row labels of DataFrame</td></tr>
  <tr><td><a href=#column><code>DataFrame.columns</code></a></td> <td>Column labels of DataFrame</td></tr>
  <tr><td><a href=#axes><code>DataFrame.axes</code></a></td> <td>Label values of rows and columns in the DataFrame</td></tr>
  <tr><td><a href=#dtype><code>DataFrame.dtypes</code></a></td> <td>Data types for each column of DataFrame</td></tr>
  <tr><td><a href=#size><code>DataFrame.size</code></a></td> <td>Total number of elements in a DataFrame</td></tr>
  <tr><td><a href=#shape><code>DataFrame.shape</code></a></td> <td>Dimensions of DataFrame ( Number of rows, Number of columns )</td></tr>
  <tr><td><a href=#ndim><code>DataFrame.ndim</code></a></td> <td>No. of Dimensions ( 1D, 2D, 3D )</td></tr>
  <tr><td><a href=#empty><code>DataFrame.empty</code></a></td> <td>Check whether DataFrame is empty or not</td></tr>
  <tr><td><a href=#T><code>DataFrame.T</code></a></td> <td>Change the rows into columns and columns into rows</td></tr>  
  <tr><td><a href=#value><code>DataFrame.values</code></a></td> <td>Values of DataFrame in the form of NumPy array</td></tr>  
</table>

<h3 name=index><code>DataFrame.index</code></h3>

```python
print(df.index)

# By default it automatically creates a RangeIndex(start=0, stop=len(df), step=1)
# We can manually add index by passing list to index parameter i.e. index = [1, 2, 3]
# We can also set some existing column as an index i.e index = 'City'
```

<h3 name=column><code>DataFrame.columns</code></h3>

```python
print(df.columns)
```

<h3 name=axes><code>DataFrame.axes</code></h3>

```python
print(df.axes)
```

<h3 name=dtype><code>DataFrame.dtypes</code></h3>

```python
print(df.dtypes)
```

<h3 name=size><code>DataFrame.size</code></h3>

```python
print(df.size)
```

<h3 name=shape><code>DataFrame.shape</code></h3> 

```python
# Dimensions of the dataframe:
print(df.shape)

# Extract only the total number of rows in a dataframe:
print(df.shape[0])

# Extract only the total number of columns in a dataframe:
print(df.shape[1])
```            

<h3 name=ndim><code>DataFrame.ndim</code></h3>

```python
print(df.ndim)
```

<h3 name=empty><code>DataFrame.empty</code></h3> 

```python
print(df.empty)
```

<h3 name=T><code>DataFrame.T</code></h3>

```python
print(df.T)
```

<h3 name=value><code>DataFrame.values</code></h3>

```python
print(df.values)
```
