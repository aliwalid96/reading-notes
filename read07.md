# Python Scope & the LEGB Rule:

 Local, Enclosing, Global, and Built-in
 ### what is the scope 
 In programming, the scope of a name defines the area of a program in which you can unambiguously access that name, such as variables, functions, objects, and so on. A name will only be visible to and accessible by the code in its scope.
 .

 kind of scope :
 1. Global scope: The names that you define in this scope are available to all your code.

2. Local scope: The names that you define in this scope are only available or visible to the code within the scope.

## Using the LEGB Rule for Python Scope
1. Local (or function) scope is the code block or body of any Python function or lambda expression

2. Enclosing (or nonlocal) scope is a special scope that only exists for nested functions.

3. Global (or module) scope
is the top-most scope in a Python program, script, or module

4. Built-in scope is a special Python scope that’s created or loaded whenever you run a script or open an interactive session.

The local scope or function scope is a Python scope created at function calls. Every time you call a function, you’re also creating a new local scope.

Enclosing or nonlocal scope is observed when you nest functions inside other functions.

builtins: The Built-In Scope
The built-in scope is a special Python scope that’s implemented as a standard library module named builtins in Python
### Modifying the Behavior of a Python Scope

Bringing Names to Scope With import
When you write a Python program, you typically organize the code into several modules. For your program to work, you’ll need to bring the names in those separate modules to your __main__ module. To do that, you need to import the modules or the names explicitly. This is the only way you can use those names in your main global Python scop

Using Scope Related Built-In Functions
There are many built-in functions that are closely related to the concept of Python scope and namespaces. In previous sections, you’ve used dir() to get information on the names that exist in a given scope. 

## Big O notation is the time and space complexity 
is quantifying and comparing the algorithem
is the worest case senario
