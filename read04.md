# Classes and Objects

Objects are an encapsulation of variables and functions into a single entity. Objects get their variables and functions from classes. Classes are essentially a template to create your objects.
 ## when you create an class which can have multiple    variable and function tou can creat an object Which let you access the variable and function fron the class


```class MyClass:
    variable = "blah"

    def function(self):
        print("This is a message inside the class.")

myobjectx = MyClass()

myobjectx.variable
```
in this code the class named MyClass
and has some variable and function we created an object named myobjectx
and by it we can acess all variable and data 
like 
myobjectx.variable name or function name

### and for sure you cane create multiple object for the same class 

# Thinking Recursively in Python

This is the typical structure of a recursive algorithm. If the current problem represents a simple case, solve it. If not, divide it into subproblems and apply the same strategy to them.

## Recursive Functions in Python

 A recursive function is a function defined in terms of itself via self-referential expressions.

This means that the function will continue to call itself and repeat its behavior until some condition is met to return a result. All recursive functions share a common structure made up of two parts: base case and recursive case.

# Python Testing with pytest: Fixtures and Coverage

I review two features of pytest that I haven't had a chance to cover yet: fixtures and code coverage, which will (I hope) convince you that pytest is worth exploring and incorporating into your work
## Fixtures
When you're writing tests, you're rarely going to write just one or two. Rather, you're going to write an entire "test suite", with each test aiming to check a different path through your code. In many cases, this means you'll have a few tests with similar characteristics, something that pytest handles with "parametrized tests".



