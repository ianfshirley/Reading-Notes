## Data Analysis

### What is Jupyter Lab

- JupyterLab is a next-generation web-based user interface for Project Jupyter.
- It allows you to work with documents and activities such as Jupyter notebooks, text editors, terminals and custom components in a flexible, integrated, and extensible manner
- Jupyter notebooks are a new way to work easily with data and code, seamlessly together.
  - Command mode is designed for easily navigating and changing the framework of your notebook
    - that framework is composed of cells, which keep your data, thoughts, and code in little containers
    - keyboard shortcuts:
      - a - add a cell above
      - b - add a cell below
      - c - copy a cell
      - v - paste
      - x - cut a cell
      - dd - delete a cell
      - z - undo
      - Shift + z - redo
      - y - change format of cell into code
      - m - change format of cell into markdown
  - Edit mode - press 'enter' to edit the currently active cell
    - some markdown tips I didn't know:
      - `inline code` by wrapping the code in backticks
      - ```
        for a code block, 3 backticks on the line above and 3 backticks on the line below
        ```
      - for equations, such as $x^2$, wrap the text between $ symbols
  - To run the code in the active cell (after first typing 'y' to switch to code format):
    - shift + enter
    - output is printed under the cell
    - the whole notebook runs on the same 'kernel', so if you update the value for a variable in a later cell, it will update its value in previous cells if you run the previous cell's code again

### Numpy Tutorial

- A commonly used Python data analysis package. By using NumPy, you can speed up your workflow and interface iwth other packages in the Python ecosystem, like scikit-learn, that use NumPy under the hood.
- It's a library consisting of multidimensional array objects and a collection of routines for processing those arrays.
- NumPy works with 2-dimensional arrays
  - the number of dimensions is called the rank, and each dimension is an axis.
  - in 2-dimensional arrays, the rows are the first axis and the columns are the second axis
  - create the array by using the numpy.array function (after importing numpy)
    - one limitation is that all the data types must be the same, so if you want your data as integers or floats, you'll have to leave off the header row that consist of strings (slice the row)
  - check the number of rows and columns by using the 'shape' property of NumPy arrays (list_name.shape)
  - Indexing:
    - NumPy arrays are 0 indexed
    - We can retrieve the value from row 3 and column 4 in `numpy_arr` like this: `numpy_arr[2, 3]`
    - we can also use the colon to slice/retrieve multiple values. 
  

### Sources

[Overview - Jupyter Lab](https://jupyterlab.readthedocs.io/en/stable/getting_started/overview.html)<br>
[How to Use Jupyter Lab](https://www.youtube.com/watch?v=A5YyoCKxEOU&feature=emb_imp_woyt)<br>
[NumPy Tutorial: Data Analysis with Python](https://www.dataquest.io/blog/numpy-tutorial-python/)<br>
[NumPy Tutorial](https://www.tutorialspoint.com/numpy/index.htm)<br>