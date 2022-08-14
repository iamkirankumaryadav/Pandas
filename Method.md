# `Method`

### `DataFrame.head(n)` : Displays top n rows from the DataFrame.

```python
# Default value for n is 5
df.head(n=10)
```          

### `DataFrame.tail(n)` : Displays bottom n rows from the DataFrame.

```python
# Default value for n is 5
df.tail(n=10)
```          

### `DataFrame.info()` : Represents the summary of the DataFrame:

1. Number of rows
2. Number of columns
3. Data type
4. Number of Non Null rows
5. Memory usage by the data frame

```python
df.info()
```                 

### `DataFrame.query()` : Filter DataFrame by query conditions.

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

### `Series.value_counts()` : Represents an object containing counts of unique values.

```python
df['City'].value_counts(normalize=False, sort=True, ascending=False, bins=None, dropna=True)
```            

### `Series.sort_values()` : Sort values along either axis.

```python   
df['Age'].sort_values(axis=0, ascending=True, inplace=False, kind='quicksort', na_position='last')
```            

### `DataFrame.sort_values()` : Sort value by Column values.

```python
df.sort_values(by=['Age', 'Salary'], axis=0, ascending=[True, True], inplace=False, kind='quicksort', na_position='last')
```

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

### `DataFrame.set_index()` : Set other column as an index.

```python
# Set column "City" as an index:
df.set_index(keys='City', drop=True, append=False, inplace=False, verify_integrity=False)

# Set multi index:
df.set_index(keys=['City', 'State'], drop=True, inplace=False)
```

### `DataFrame.reset_index()` : Returns a DataFrame with the default `integer based` index.

```python
df.reset_index(level=None, drop=False, inplace=False, ...)
```

### `DataFrame.sort_index()` : Sort objects by a label along the axis.

- `axis=0` represents rows and `axis=1` represents columm.

```python
df.sort_index(axis=0, level=None, ascending=True, inplace=False, by=None)
```

### `DataFrame.fillna()` : Fill or replace missing values in DataFrame.

```python
# DataFrame.fillna()
df.fillna('🌞')

# DataFrame.Series.fillna()
df['Sales'].fillna(0)
```

### `DataFrame.dropna()` : Drop rows or columns that contains NaN values.

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

# DataFrame `Groupby`

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

# Dataframe `Reshaping` : 

- Changing the structure of DataFrame to represent data in desired form.

![Stack and Unstack](../Image/Reshaping.png)

### `DataFrame.stack()` : Represents a taller DataFrame. 

- `Stacking` increases the height of data frame.
- `stack()` method helps us to move the columns into row values.

### `DataFrame.unstack()` : Represents a wider DataFrame.

- `Unstacking` decreases the height of data frame.
- `unstack()` method helps us to move the row values to seperate columns. 
