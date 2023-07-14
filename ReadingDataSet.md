# Code Explanation

This repository contains code snippets demonstrating the usage of various Pandas functions for data analysis. The code snippets are organized in a logical order and cover different aspects of working with data using Pandas.

## Code Snippets

### 1. Creating a DataFrame

```python
import pandas as pd

data = {'apples': [4, 5, 7, 8], 'oranges': [2, 7, 1, 9]}
df = pd.DataFrame(data)
df = pd.DataFrame(data, index=['Bharat', 'Rabin', 'Haaku', 'Milan'])
```

Creates a DataFrame using a Python dictionary and assigns it to the variable `df`. The DataFrame has two columns: 'apples' and 'oranges', and it also specifies custom row indices.

### 2. Accessing Data

```python
df.loc['Milan']
```

Accesses the row with the index label 'Milan' in the DataFrame `df` and returns the corresponding data.

### 3. Reading Data from a CSV File

```python
df = pd.read_csv('titanic.csv')
```

Reads data from a CSV file named 'titanic.csv' and assigns it to the DataFrame `df`.

### 4. Reading Data from a CSV File with Index Column

```python
df = pd.read_csv('titanic.csv', index_col=0)
```

Reads data from a CSV file named 'titanic.csv' and uses the first column as the index column when creating the DataFrame `df`.

### 5. Printing Information about the DataFrame

```python
df.info()
```

Prints information about the DataFrame `df`, including the number of rows, number of columns, column names, and data types.

### 6. Getting the Size of the DataFrame

```python
df.shape
```

Returns the dimensions of the DataFrame `df` as a tuple containing the number of rows and columns.

### 7. Generating Descriptive Statistics

```python
df.describe()
```

Generates descriptive statistics for the integer columns in the DataFrame `df`, including count, mean, standard deviation, minimum value, 25th percentile, median, 75th percentile, and maximum value.

### 8. Descriptive Statistics for a Specific Column

```python
df['Survived'].describe()
```

Provides descriptive statistics for the 'Survived' column in the DataFrame `df`, including count, mean, standard deviation, minimum value, 25th percentile, median, 75th percentile, and maximum value.

## Conclusion

These code snippets showcase different functionalities of Pandas library for data analysis, including creating a DataFrame, accessing data, reading data from a CSV file, printing information about the DataFrame, calculating descriptive statistics, and more.