## File IO & Exceptions

### Read & Write Files in Python

##### What is a File?

- At its core, a file is a contiguous set of bytes used to store data. It can be as simple as a text file or as complicated as an executable program.
- Files on most modern file systems are composed of three main parts:
  - Header: metadata about the contents of the file (file name, size, type, etc.)
  - Data: the contents of the file
  - End of File (EOF): special character that indicates the end of the file

##### Opening and Closing a File in Python

- Opening a file is done by invoking the built-in open() function, which has one required argument, the file path.
- It's important to close files when you're done with them (resource leaks).
- Best way to close files is the 'with' statement, it will close the file once it leaves the code block.

##### Reading and Writing Opened Files

- .read(size=-1) - reads from file based on number of 'size' bytes
- .readline(size=-1) - reads at most 'size' number of characters from the line. contines to end of line and wraps back around
- readlines() - reads the remaining lines form the file object and returns them as a list

### Exceptions in Python

- Exception errors are when sytactically correct Python code results in an arror. 
- You can use 'raise' to throw an exception if a condition occurs. 
  Example:
  x = 10
  if x > 5:
    raise Exception('x should not exceed 5. The value of x was: {}'.format(x))

- 'raise' allows you to throw an exception at any time.
- 'assert' enables you to verify if a certain condition is met and throw an exception if it isn’t.
- In the 'try' clause, all statements are executed until an exception is encountered.
- 'except' is used to catch and handle the exception(s) that are encountered in the try clause.
- 'else' lets you code sections that should run only when no exceptions are encountered in the try clause.
- 'finally' enables you to execute sections of code that should always run, with or without any previously encountered exceptions.

### Sources

[Read & Write Files in Python](https://realpython.com/read-write-files-python/)<br>
[Exceptions in Python](https://realpython.com/python-exceptions/)<br>
[Read & Write Files in Python - Companion Video](https://realpython.com/courses/reading-and-writing-files-python/)<br>
[Reading and Writing Files in Python Quiz](https://realpython.com/quizzes/read-write-files-python/)<br>