# Page 1

We can use \*\*dict to unpack the dict values and keys

```python
mydict = {'a': 1, 'b': 2}

SomeClass(**mydict) # Equivalent to : SomeClass(a=1, b=2)
```

```python
Python 3.10.10 (main, Mar  5 2023, 22:26:53) [GCC 12.2.1 20230201] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> import numpy
>>> import sqlalchemy
>>> class Creator:
...     def __init__(self, creator_name="", creator_name_type=""):
...             self.creator_name = creator_name
...             self.creator_name_type = creator_name_type
... 
>>> dict_creator = {"creator_name": "Mauricio Caroca", "creator_name_type": "Personal"}
>>> person = Creator(dict_creator.values())
>>> person
<__main__.Creator object at 0x7f89a58dfaf0>
>>> person.creator_name
dict_values(['Mauricio Caroca', 'Personal'])
>>> person.creator_name_type
''
>>> person2 = Creator(val for val in dict_creator.values())
>>> person2.creator_name
<generator object <genexpr> at 0x7f897ead2ea0>
>>> person = Creator(**dict_creator)
>>> person.creator_name
'Mauricio Caroca'
>>> person.creator_name_type
'Personal'
>>> 

```

<table data-view="cards"><thead><tr><th></th><th></th><th></th></tr></thead><tbody><tr><td></td><td>lkjfsghaag</td><td></td></tr><tr><td></td><td>asfdhafseeh</td><td></td></tr><tr><td></td><td>asdfhsdfgh</td><td></td></tr></tbody></table>
