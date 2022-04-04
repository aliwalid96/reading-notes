# JupyterLab

JupyterLab enables you to work with documents and activities such as Jupyter notebooks, text editors, terminals, and custom components in a flexible, integrated, and extensible manner. 


jupeter notebook is like a frame work and you can handle it by some command 
to add cells above with a
add acells below with b 
copy  cell by c 
paste by v 
delete by d d
undo by z 
redo with shift with z 
code format with y 
markdown format with m

you can handle markdown cells by mark downconsipt

and for python cells if you have a lot of cells 
and the code depend on each other you should run the cells frequentlly 

## NumPy Tutorial: Data Analysis with Python

Creating A NumPy Array

We can create a NumPy array using the numpy.array function. If we pass in a list of lists, it will automatically create a NumPy array with the same number of rows and columns. Because we want all of the elements in the array to be float elements for easy computation, we’ll leave off the header row, which contains strings. 

~~~
import csv
with open("winequality-red.csv", 'r') as f:
    wines = list(csv.reader(f, delimiter=";"))
import numpy as np
wines = np.array(wines[1:], dtype=np.float)
~~~
Import the numpy package.
Pass the list of lists wines into the array function, which converts it into a NumPy array.
Exclude the header row with list slicing.
Specify the keyword argument dtype to make sure each element is converted to a float. We’ll dive more into what the dtype is later on.
