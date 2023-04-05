# `Method`

<table>
      <tr><th><h3>Method</h3></th><th><h3>Description</h3></th></tr>
      <tr><td><a href=#head><code>DataFrame.head(n)</code></a></td><td>Top n rows of DataFrame</td></tr>
      <tr><td><a href=#tail><code>DataFrame.tail(n)</code></a></td><td>Bottom n rows of DataFrame</td></tr>
      <tr><td><a href=#sample><code>DataFrame.sample(n)</code></a></td><td>Random n rows of DataFrame</td></tr>
      <tr><td><a href=#info><code>DataFrame.info(n)</code></a></td><td>Summary of DataFrame</td></tr>
      <tr><td><a href=#query><code>DataFrame.query()</code></a></td><td>Filter DataFrame by query conditions</td></tr>
      <tr><td><a href=#count><code>DataFrame.value_counts()</code></a></td><td>Represents an object containing counts of unique values</td></tr>      
      <tr><td><a href=#index><code>DataFrame.sort_index()</code></a></td><td>Sort the DataFrame by index</td></tr>
      <tr><td><a href=#value><code>DataFrame.sort_values()</code></a></td><td>Sort the DataFrame values</td></tr>
      <tr><td><a href=#set><code>DataFrame.set_index()</code></a></td><td>Set other column as DataFrame index</td></tr>            
      <tr><td><a href=#reset><code>DataFrame.reset_index()</code></a></td><td>Reset the DataFrame index</td></tr>     
      <tr><td><a href=#fillna><code>DataFrame.fillna()</code></a></td><td>Fill NaN | missing values in DataFrame</td></tr>     
      <tr><td><a href=#dropna><code>DataFrame.dropna()</code></a></td><td>Drop rows or columns that contains NaN values</td></tr>     
      
</table>

### `Series.str` : Perform string operations.

String handling is done by using attribute `str`: Access values of series as `strings` and apply several methods on that.

```python
# Series.str.contains()
df['City'].str.contains('Mumbai')

# Series.str.startswith()
df['LastName'].str.startswith('Yadav')

# Series.str.isnumeric()
df['Pincode'].str.isnumeric()
```          

<h3 name=head><code>DataFrame.head(n)</code></h3> 

```python
# Default value for n is 5
df.head(n=10)
```          

### `DataFrame.tail(n)` 

```python
# Default value for n is 5
df.tail(n=10)
```          

### `DataFrame.info()` 

1. Number of rows
2. Number of columns
3. Data type
4. Number of Non Null rows
5. Memory usage by the data frame

```python
df.info()
```                 

### `DataFrame.query()` 

```python
df.query("Country == 'India' and State in ('Maharashtra', 'Hyderabad') and Year > 2021")

# Query using variable name:
Name = input('Enter Employee Name:')
JoiningYear = int(input('Enter Joining Year:'))
df.query("EmployeeName == @Name and YearofJoining == @JoiningYear" )

# Query rows using list of values:
ITState = ['Hyderabad', 'Bangalore', 'Chennai']
df.query("Country == 'India' and State in @ITState")
```

### `Series.value_counts()` 

```python
df['City'].value_counts(normalize=False, sort=True, ascending=False, bins=None, dropna=True)
```            

### `DataFrame.sort_index()` 

- `axis=0` represents rows and `axis=1` represents columm.

```python
df.sort_index(axis=0, level=None, ascending=True, inplace=False, by=None)
```

### `Series.sort_values()` 

```python   
# Sort by Axis:
df['Age'].sort_values(axis=0, ascending=True, inplace=False, kind='quicksort', na_position='last')

# Sort by Column Names:
df.sort_values(by=['Age', 'Salary'], axis=0, ascending=[True, True], inplace=False, kind='quicksort', na_position='last')
```  

### `DataFrame.set_index()` 

```python
# Set column "City" as an index:
df.set_index(keys='City', drop=True, append=False, inplace=False, verify_integrity=False)

# Set multi index:
df.set_index(keys=['City', 'State'], drop=True, inplace=False)
```

### `DataFrame.reset_index()` 

```python
df.reset_index(level=None, drop=False, inplace=False, ...)
```

### `DataFrame.fillna()` 

```python
# DataFrame.fillna()
df.fillna('🌞')

# DataFrame.Series.fillna()
df['Sales'].fillna(0)
```

### `DataFrame.dropna()` 

```python
# DataFrame.dropna()
df.dropna()

# DataFrame.Series.dropna()
df['Sales'].dropna()

# Drop rows
df.dropna(axis=0)

# Drop if any attribute value is NaN
df.dropna(axis=0, how='any')

# Drop if all the attribute values are NaN
df.dropna(axis=0, how='all')

# Drop columns
df.dropna(axis=1)
```
