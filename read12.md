# pandas

we import its classes by 
import numpy as np
import pandas as pd


To load the pandas package and start working with it, import the package. The community agreed alias for pandas is pd, so loading pandas as pd is assumed standard practice for all of the pandas documentation.



To manually store data in a table, create a DataFrame. When using a Python dictionary of lists, the dictionary keys will be used as column headers and the values in each list as columns of the DataFrame.


A DataFrame is a 2-dimensional data structure that can store data of different types (including characters, integers, floating point values, categorical data and more) in columns. It is similar to a spreadsheet, a SQL table or the data.frame in R.


We can do this on the DataFrame by selecting the Age column and applying max():

pandas provides the read_csv() function to read data stored as a csv file into a pandas DataFrame.

Getting data in to pandas from many different file formats or data sources is supported by read_* functions.
## select data from dataframe
To select a single column, use square brackets [] with the column name of the column of interest.

