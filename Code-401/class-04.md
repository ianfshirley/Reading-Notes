### Classes & Objects

- Objects are an encapsulation of variables and function into a single entity. Objects get their variables and functions from classes. Classes are essentially a template to create your objects.
- To create a basic class:
  class MyClass:
    variable = "blah"

    def function(self):
        print("This is a message inside the class.")
- Access Object Variables (this will print "blah" in the shell):
  class MyClass:
    variable = "blah"

    def function(self):
        print("This is a message inside the class.")

  myobjectx = MyClass()

  print(myobjectx.variable)
- Access Object Functions:
  myobjectx.function()
- The  __init__() function is a special function that is called when the class is being initiated. It's used for assigning values in a class.

### Thinking Recursively

- Recursive functions continue to call themselves and repeat their behavior until some condition is met to return a result. All recursive functions share a common structure made up of two parts: base case and recursive case. Doing it this way rather than iteratively will break up a large problem into multiple smaller problems.
  - **Base case:** the simple sub-problems that can be solved without further division. Also, if the base case is met and a return is given, no recursion is needed.
  - **Recursive case:** the conditions that will cause the function to keep calling itself until a base case is met 
- You need to maintain state. There are two ways of doing this:
  - Thread the state through each recursive call so that the current state is part of the current call's execution context
  - Keep the state in the global scope
- Recursive Data Structures in Python
  - A data structure is recursive if it can be defined in terms of a smaller version of itself. Examples include lists, sets, dicts...

### Pytest Fixtures and Coverage

- Fixtures provide defined, reliable and consistent context for tests.
- Coverage is making sure that you have tests that will cover all of your code.

### Sources

[Classes & Objects](https://www.learnpython.org/en/Classes_and_Objects)<br>
[Thinking Recursively](https://realpython.com/python-thinking-recursively/)<br>
[Pytest Fixtures and Coverage](https://www.linuxjournal.com/content/python-testing-pytest-fixtures-and-coverage)<br>
[Pytest Fixtures](https://docs.pytest.org/en/latest/explanation/fixtures.html)<br>