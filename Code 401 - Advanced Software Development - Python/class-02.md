## Testing and Modules

### In Tests We Trust - TDD with Python

- Unit tests are pieces of code to exercise the input, output and behavior of your code. Test-Driven Development is a strategy to think about the tests first.
- Another thing to think about is the structure. A convention widely used is AAA: Arrange, Act, Assert
  - Arrange - organize the data needed to execute that piece of code (input)
  - Act - execute the code being tested (behavior)
  - Assert - after executing the code, check if the result (output) is what you were expecting
- The Cycle - three steps:
  - Write a unit test and make it fail
  - write the feature and make the test pass
  - refactor the code
- The advantage is that TDD will cause you to make the software design first, and it will be more reliable if it is designed with the tests already in mind

### If __name__ = "__main__" - What does it do?

- Before executing code, Python interpreter reads the source file and defines a few special/global variables. If it's running that module/source file as the main program, it sets the __name__ variable to have a value of "__main__". If the file is being imported from another module, the __name__ variable will be set to the module's name.
- Anything at indentation level 0 gets executed, but anything in the 'if __name__ = "__main__"' code block will only run if that module is the entry point into your program.

### Introduction to Recursion

- What is Recursion?
  - The process in which a function calls itself directly or indirectly. The corresponding function is called a recursive function.
  - A recursive function solves a problem by calling a copy of itself and solving smaller sub-problems.
- Need of Recursion
  - This technique can help reduce the length of our code and make it easier to read and write.
- Properties of Recursion
  - Performing the same operation multiple times with different inputs
  - In every step, we try smaller inputs to make the problem smaller
  - Base condition is needed to stop the recursion, otherwise an infinite loop will occur
- Direct vs. Indirect Recursion
  - direct recursion is when a function calls itself
  - indirect recursion is when a function calls another function

### Sources

[In Tests We Trust - TDD with Python](https://code.likeagirl.io/in-tests-we-trust-tdd-with-python-af69f47e6932)<br>
[If name equals main](https://www.geeksforgeeks.org/what-does-the-if-__name__-__main__-do/)<br>
[Recursion](https://www.geeksforgeeks.org/introduction-to-recursion-data-structure-and-algorithm-tutorials/)<br>
[What on Earth is Recursion](https://www.youtube.com/watch?v=Mv9NEXX1VHc)<br>
[Python Modules and Packages Companion Video](https://realpython.com/courses/python-modules-packages/)<br>
[Google for Education: Python Lists](https://developers.google.com/edu/python/lists)<br>
[Google for Education: Python Strings](https://developers.google.com/edu/python/strings)<br>
[Python Modules and Packages](https://realpython.com/python-modules-packages/)<br>
[Pytest Documentation](https://docs.pytest.org/en/latest/)<br>
[PyTest Tutorial](https://www.guru99.com/pytest-tutorial.html)<br>