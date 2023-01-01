## Ten Thousand #2

### Python Scope & the LEGB Rule: Resolving Names in Your Code

- Global Scope: 
  - The names that you define in this scope are available to all your code
- Local Scope:
  - The names that you define in this scope are only available or visible to the code within the scope.
- Using the LEGB rule for Python Scope
  - Local (or function) Scope
    - The code block or body of any Python function or Lambda expression
    - The scope is created at function call, not function definition, so there will be as many local scopes as function calls
  - Enclosing (or nonlocal) Scope
    - Only exists for nested functions. If the local scope is an inner or nested function, the enclosing scope is the scope of the outer or enclosing function
  - Global (or module) Scope
    - names in this Python scope are visible from everywhere in your code
  - Built-in Scope
    - Created or loaded whenever you run a script or open an interactive session
    - Contains names such as keywords, functions, exceptions and other attributes that are built into Python
    - visible from everywhere in your code

### Sources

[Python Scope & the LEGB Rule: Resolving Names in Your Code](https://realpython.com/python-scope-legb-rule/)<br>