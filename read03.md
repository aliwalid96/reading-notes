## Reading and Writing Files in Python
the file is : file is a contiguous set of bytes used to store data. This data is organized in a specific format and can be anything as simple as a text file or as complicated as a program executable

the path for file is
The file path is a string that represents the location of a file

### Character Encodings
is cinvert the file from machine language to human language
# Opening and Closing a File in Python
first step oben the file by 
file = open('dog_breeds.txt')

### You should always make sure that an open file is properly closed
file name .close()

The with statement automatically takes care of closing the file once it leaves the with block, even in cases of error. I highly recommend that you use the with statement as much as possible, as it allows for cleaner code and makes handling any unexpected errors easier for you.

some alphabet has special meaning 

'r'	Open for reading (default)
'w'	Open for writing, truncating (overwriting) the file first
'rb' or 'wb'	Open in binary mode (read/write using byte data)



## Python Exceptions
occur when the parser detects an incorrect statement
### Raising an Exception
We can use raise to throw an exception if a condition occurs. The statement can be complemented with a custom exception
### The AssertionError Exception
### The try and except Block: Handling Exceptions
 Python executes code following the try statement as a “normal” part of the program. The code that follows the except statement is the program’s response to any exceptions in the preceding try clause.
 The else Clause
In Python, using

 the else statement, you can instruct a program to execute a certain block of code only in the absence of exceptions.

Diagram of try, except, and else statements in Python
