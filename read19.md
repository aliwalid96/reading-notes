# Django Tutorial Part 3: Using models

Django web applications access and manage data through Python objects referred to as models. Models define the structure of stored data

## Designing the LocalLibrary models

Once we've decided on our models and field, we need to think about the relationships. Django allows you to define relationships that are one to one (OneToOneField), one to many (ForeignKey) and many to many (ManyToManyField).


he diagram also shows the relationships between the models, including their multiplicities. The multiplicities are the numbers on the diagram showing the numbers (maximum and minimum) of each model that may be present in the relationship.

## Model definition
Models are usually defined in an application's models.py file. They are implemented as subclasses of django.db.models.Model, and can include fields, methods and metadata. The code fragment below shows a "typical" model, named MyModelName


### Fields
A model can have an arbitrary number of fields, of any type — each one represents a column of data that we want to store in one of our database tables.

### COMMON FIELD TYPES
1. CharField
2. TextField
3. IntegerField
4. DateField
4. EmailField
5. ForeignKey
6. ManyToManyField


A model can also have methods.

Minimally, in every model you should define the standard Python class method __str__() to return a human-readable string for each object. 


Once you've defined your model classes you can use them to create, update, or delete records, and to run queries to get all records or particular subsets of records


# Django Tutorial Part 4: Django admin site


First, open admin.py in the catalog application (/locallibrary/catalog/admin.py). It currently looks like this — note that it already 
~~~
imports django.contrib.admin

~~~

Creating a superuser
In order to log into the admin site, we need a user account with Staff status enabled.

~~~
python3 manage.py createsuperuser

python3 manage.py runserver

~~~

To login to the site, open the /admin URL (e.g. http://127.0.0.1:8000/admin) 
    