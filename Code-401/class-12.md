## Pandas

### Pandas in 10

- To start, import numpy and pandas:
  - `import numpy as np`
  - `import pandas as pd`
- To manually store data in a table, create a DataFrame
- A dataframe is a 2D data structure that can store different data types in columns (similar to a spreadsheet, SQL table or the `data.frame` in R)
- Each column in a `DataFrame` is a `Series`
- To select the column, use the column label in between square brackets:
  - `df["age"]` to select just the column labeled "age"
  - you can also use dot notation in some cases: df.age
- There are many built-in methods you can use to do things with a dataframe or series. 
- In order to create plots: `import matplotlib.pyplot as plt`



### Sources

[Pandas in 10](https://pandas.pydata.org/pandas-docs/stable/user_guide/10min.html)<br>
[Pandas - Getting Started](https://pandas.pydata.org/pandas-docs/stable/getting_started/intro_tutorials/index.html)<br>
[Real Python - Pandas Tutorial](https://realpython.com/learning-paths/pandas-data-science/)<br>
[What is Pandas](https://www.youtube.com/watch?v=dcqPhpY7tWk&t=391s)<br>
[Master Pandas](https://towardsdatascience.com/be-a-more-efficient-data-scientist-today-master-pandas-with-this-guide-ea362d27386)<br>