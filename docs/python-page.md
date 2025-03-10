# Python

## LIBRARIES

`from math import pi, cos`
or `import math as m —> m.pi, m.cos`

```python
anaconda
    **numpy**, scipy, **scikit-learn**, **keras**, 
scrapy, beautifulsoup4, nltk, gensim
django, **flask**, flask-cors, git, gunicorn, mysql-connector-python
tbc: nodejs, **tensorflow**
explore: graphviz, jinja2, mongodb, sqlite, **pytorch**, 
scikit-bio, scikit-image, scikit-learn, urllib3
```

```python
import pandas as pd
df = pd.read_excel('sales_data.xlsx', sheet_name='2021')
```
```python
xls = pd.ExcelFile('path_to_file.xls')
df1 = pd.read_excel(xls, 'Sheet1')
df2 = pd.read_excel(xls, 'Sheet2')
```

### Visualization libraries:

**matplotlib**, **seaborn** (modern looking), Plotnine (ggplot2 port from R)**, bokeh** (python native, interactive), pygal (output svg), **plotly*** (dash, online also, interactive), geoplotlib, Gleam (filter & sort), missingno, folium (geo), **flourish**

## Data Analysis

### streamlit (st)

```python
import plotly.express as px //https://plotly.com/python/plotly-express/
```

## Virtual Environments (virtualenv & virtualenvwrapper)

• Conda

## Bitwise operators

- complement ~
reverse all bits → The bitwise inversion of x is defined as -(x+1)
- and &
    
    1 & 1 = 1
    
- or |
    
    1 | 1 = 1
    
- xor ^
    
    1 ^ 1 = 0 (two different then =1)
    
- left shift <<
    
    num << n (shift by n) (net gain of bits)
    
- right shift >>

## string manipulation
number of substrings: ((n)*(n+1))/2

## f strings

- leading zeros where 0 is the padding, 3 is the total places
    
    `f'{num1:03}'` 003
    
- decimal place
    
    `f'{math.pi:.4f}'` 3.1416 (nearest round)

- grouping 1,000
- hexadecimal
- character to ASCII
- percentage 0.25 / 25%

## Control flow

### break

jumps out of loop

### continue

skip & go back to continue the loop

### pass

remain in loop but doesn't execute code

---

### try

try something wrong, then will execute except block

### except <name or error>

if error specified is right, then code will execute

### finally

code execute no matter what happen, useful to close an open process eg .open() .close()

### raise

raise an exception (error) and stop program

### assert (debugging)

```python
x = "hello"
assert x == "goodbye" # False: AssertionError is raised
```

## Methods

### lambda functions

https://[realpython.com/python-lambda](http://realpython.com/python-lambda)

lambda n : "..."
```
>> sum = lambda a, b, c: a + b + c
>> sum(1, 2, 3)
6
```

### filter(function, iterables)

creates outputs that fulfil conditions 

### map(function, iterables)

list(map(function, sequence))

### functools.reduce()

```python
import functools
def add(x, y): # can assign initial value to x too
    return x + y

list = [2, 4, 7, 3]
print(functools.reduce(add, list)) ## sum of 16
```

---

### Decorators

modify function on the fly

### Classes & Objects

### init__

### main__

### name__

```python
if __name__ == "__main__":
	main()
```

## Iterators

### next__

### iter__

## Generators

### yield

function will return a generator

## Multithreading

***args**

```python
def myFun(*argv): 
    for arg in argv: 
        print (arg)
    
myFun('Hello', 'Welcome', 'to', 'GeeksforGeeks')
```

****kwargs**

```python
def myFun(**kwargs): 
    for key, value in kwargs.items():
        print ("%s == %s" %(key, value))
  
myFun(first ='Geeks', mid ='for', last='Geeks')
```

## Multithreading

## Useful functions

https://www.youtube.com/watch?v=bga3XQ0am4M&list=PLMOobVGrchXO8HG7eStbnwWkyLstTHVJo&index=1

zip()
super()
hash()
format()
enumerate()
memoryview()
pow()
repr()
strip()
round()
abs()
dir()
clear()