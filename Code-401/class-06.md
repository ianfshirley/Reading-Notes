## Ten Thousand #1

### How to Use the Random Module

- This can be used to pick a random number in a given range, pick a random element from a python list, pick a random card from a deck, flip a coin, etc.
- The Random module contains the following functions:
  - randint()
    - can be used to create random strings within a range
    - takes two numbers as its input argument: the start and end of the range
    - returns a random integer in the given range
  - random()
    - generates a random number between 0 and 1 (result can be multiplied to get a larger number)
  - choice()
    - used to select a random element from a collection object (list, set, tuple, etc.)
    - takes a collection object as its input argument
  - randrange()
    - used to select a random element from a given range
    - takes three numbers as input argument:
      - start - start of range (optional, default = 0)
      - stop - end of range (required)
      - step - specifies the incrementation (optional, default = 1)
  - shuffle()
    - takes a list as its input argument, and shuffles the elements of that list in place

### What is Risk Analysis

- In Software Testing, risk analysis is the process of identifying the risks in applications or software that you built and prioritizing them to test. After that, the process of assigning the level of risk is done. The categorization of the risks takes place, hence, the impact of the risk is calculated.
- Using risk analysis at the beginning of a project highlights the potential problem areas.
- How to perform risk analysis:
  - search for the risk(s)
  - analyze the impact of each individual risk
  - enact measures to mitigate the risk(s) identified

### Test Coverage

- A useful tool for finding untested parts of a codebase.
- Don't focus on a numerical measure of test coverage, a high % can be attained even with low quality testing.
- According to the author, you are doing enough testing if the following are both true:
  - you rarely get bugs that escape into production
  - you are rarely hesitant to change some code for fear it will cause production bugs
- Small changes in your code should not require much change in the tests

### Big O Notation

- Comparing transferring data via the internet vs via a carrier pigeon carrying a USB drive:
  - carrier pigeon is O(1) - same speed regardless of the amount of data on the USB drive
  - internet is O(n) - time needed increases linearly with increase in the amount of data
- Different steps get added
  - 2 step process O(a) + O(b) -> O(a+b)
- Drop contstants
  - if one function takes 2 steps, and another does both tasks in one step, you might think that one is O(n) and the other is O(2n). We drop the constant, both are O(n).
- Different inputs -> different variables
  - you have a function with inputs a & b
  - it wouldn't be O(n<sup>2</sup>), it would be O(a*b)
- Drop non-dominant terms
  - you havea a function with two parts, one is O(n), the other is O(n<sup>2</sup>)
  - this would not be O(n+n<sup>2</sup>), it would just be O(n<sup>2</sup>)

### Sources

[How to Use the Random Module](https://www.pythonforbeginners.com/random/how-to-use-the-random-module-in-python)<br>
[What is Risk Analysis](https://www.edureka.co/blog/risk-analysis-in-software-testing/)<br>
[Test Coverage](https://martinfowler.com/bliki/TestCoverage.html)<br>
[Big O Notation](https://www.youtube.com/watch?v=v4cd1O4zkGw)<br>
[Python Random](https://docs.python.org/3/library/random.html)<br>
[What is Dependency Injection](https://www.freecodecamp.org/news/a-quick-intro-to-dependency-injection-what-it-is-and-when-to-use-it-7578c84fa88f/)<br>