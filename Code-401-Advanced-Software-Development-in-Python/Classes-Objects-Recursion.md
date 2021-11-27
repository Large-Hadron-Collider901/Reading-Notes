## Classes and Objects

* Objects get their variables and functions from classes. 
* Classes will serve as a template to create objects
* A simple class will look like this:
**Example**:

```
class  MyClass:
    variable = "as a man thinketh in his heart, so shall be"

    def function(self):
        print("Here is a message inside of the class.")

```
* We can assign a class to an object by doing the following:
`myobjectx = MyClass()`

### Accessing Object Variables

* To access the variable inside an object, we would do the the following:

`myobjectx.variable`

* The instance below would output the string "as a man thinketh in his heart, so shall be":

`print(myobjectx.variable)`

* We can create objects of the same class which means that each object will have the same variables and functions defined, however, each object will contains independent copies of the variables define in the class.

```

class MyClass:
    variable = "as a man thinketh in his heart, so shall be"

    def function(self):
        print("Here is a message inside of the class.")

myobjectx = MyClass()
myobjecty = MyClass()

myobjecty.variable = "yackity"

# Then print out both values

print(myobjectx.variable)
print(myobjecty.variable)


```

### Accessing Object Functions

* To access functions inside of an object, we will use a notation similar to accessing a variable:

`myobjectx.function()`

* The instance above would print out: "Here is a message inside of the class."

### init()

* The `__init__()` function is a special function that we use for assigning values in a class, therefore, it is called when the class is being initiated.

```
class Person:

    def __init__(self, name):
        self.name = name

```

## Thinking Recursively In Python

* Thinking recursively is the process of solving a problem by breaking it down into smaller pieces that are trivial enough to solve.

* Iterative functions use loops whereas recursive functions uses functions that call themselves

* In a recursive function will continue to call itself and repeat it's behavior until some condition is met to return a result. 

* All recursive functions are made up of two parts: base case and recursive case.

* Base case: the condition to stop the recursion

* Recursive case: the part where th function calls on itself

```
def factorial(x):
    if x == 1: # This is the base case
        return 1
    else: # This is the recursive case
        return(x * factorial(x-1))

print(factorial(4))
```
* In the above function, we pass the integer 4 in to the function
* Then, it goes to the recursive case which gives us `return(4 * factorial(3))`
* Next, the function will call `factorial(3)` which will give us `return(3 * factorial(2))`
* This goes on until we have `x == 1` (the base case) and then the recursion will terminate
* At the end, we will have `return(4 * 3 * 2 * 1)`

### Maintaining State

* There are two ways to retain state during recursion:
1. Thread the state through each recursive call so that the current state is part of the current call's execution context
2. Keep the state in global scope

`Example 1` - `Thread the state`:
```
def sum_recursive(current_number, accumulated_sum):
    # Base case
    # Return the final state
    if current_number == 11:
        return accumulated_sum

    # Recursive case
    # Thread the state through the recursive call
    else:
        return sum_recursive(current_number + 1, accumulated_sum + current_number)

# Pass the initial state
>>> sum_recursive(1, 0)
55
```
`Example 2` - `Global Scope`:

```
# Global mutable state
current_number = 1
accumulated_sum = 0


def sum_recursive():
    global current_number
    global accumulated_sum
    # Base case
    if current_number == 11:
        return accumulated_sum
    # Recursive case
    else:
        accumulated_sum = accumulated_sum + current_number
        current_number = current_number + 1
        return sum_recursive()


>>> sum_recursive()
55
```

### Recursive Data Structures

* A data structure is recursive if it can be defined in terms of a smaller version of itself. 

* A list is an example of a recursive data structure.

* Starting with an empty list, you can generate any list by recursively applying the attach_head function

* Other recursive data structures include: set, tree, dictionary, etc.

## Testing In Python

* Run the following command in your command line: `pip install -U pytest`

* Below is an example of a test function:
```
# content of test_sample.py
def func(x):
    return x + 1


def test_answer():
    assert func(3) == 5
```
* We can use the `assert` statement to verify test expectations. 

* To execute the function, run `pytest`.

* `pytest` will run all files of the form `test_*.py` or `*_test.py`

* Use the `raises` helper to assert that some code raises an exception:
```
# content of test_sysexit.py
import pytest


def f():
    raise SystemExit(1)


def test_mytest():
    with pytest.raises(SystemExit):
        f()
```
* To execute the test function with "quiet" reporting mode, run: `pytest -q test_sysexit.py`

* The `-q/--quiet` flag keeps the output brief

* To group multiple tests together, we can put them in a class:

```
# content of test_class.py
class TestClass:
    def test_one(self):
        x = "this"
        assert "h" in x

    def test_two(self):
        x = "hello"
        assert hasattr(x, "check")
```
* In order for pytest to discover all of the tests, make sure to prefix class name with `Test `

* We can run the module by passing it's filename: `pytest -q test_class.py`










**Reading Sources**: [Classes-and-Objects](https://www.learnpython.org/en/Classes_and_Objects)
[Thinking-Recursively-in-Python](https://realpython.com/python-thinking-recursively/)
[Python-Testing-with-pytest:-Fixtures-and-Coverage](https://www.linuxjournal.com/content/python-testing-pytest-fixtures-and-coverage)