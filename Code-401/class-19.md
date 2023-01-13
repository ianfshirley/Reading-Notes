## Automation


### Regex

- To use the regex (regular expressions) library in Python, `import re`. The library contains several useful functions (compile, search, match, fullmatch, etc.) to find things in text that match the regex pattern. There are so many different symbols and characters with different meanings, I'm not putting them all into notes. I will look up the Python re documentation, regex101.com or ask chatGPT whenever I need to use regex.

### shutil

- The shutil module includes high-level file operations such as copying and archiving.
- copyfile() copies the contents of the source to the destination and raises IOError if it does not have permission to write to the destination file.
- shutil includes three functions for working with directory trees. To copy a directory from one place to another, use copytree(). It recurses through the source directory tree, copying files to the destination. The destination directory must not exist in advance.
- The which() function scans a search path looking for a named file. The typical use case is to find an executable program on the shell’s search path defined in the environment variable PATH.

### Automation Ideas

- automatically move files
- automatically move folders and rename files
- calculate compound interest


### Sources

[Python Regular Expressions Tutorial](https://www.datacamp.com/tutorial/python-regular-expression-tutorial)<br>
[shutil](https://pymotw.com/3/shutil/)<br>
[Automation Ideas](https://www.youtube.com/watch?v=qbW6FRbaSl0&t=69s)<br>
[Automating Your Browser and Desktop Apps](https://www.youtube.com/watch?v=dZLyfbSQPXI)<br>
[Watchdog](https://pythonhosted.org/watchdog/)<br>