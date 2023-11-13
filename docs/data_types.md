# Python Data Types

## Numbers

### Integers

```python
>>> 1
1
>>> 2
2
>>> 3
3
```

### Floats

```python
>>> 1.0
1.0
>>> 2.0
2.0
>>> 3.0
3.0
```

### Complex

```python
>>> 1 + 2j
(1+2j)
>>> 2 + 3j
(2+3j)
>>> 3 + 4j
(3+4j)
```

## Strings

```python
>>> 'Hello World'
'Hello World'
>>> "Hello World"
'Hello World'
>>> '''Hello World'''
'Hello World'
```

## Booleans

```python
>>> True
True
>>> False
False
```

## Lists

```python
>>> [1, 2, 3]
[1, 2, 3]
>>> ['a', 'b', 'c']
['a', 'b', 'c']
>>> [1.0, 2.0, 3.0]
[1.0, 2.0, 3.0]
>>> [1 + 2j, 2 + 3j, 3 + 4j]
[(1+2j), (2+3j), (3+4j)]
```

## Tuples

```python
>>> (1, 2, 3)
(1, 2, 3)
>>> ('a', 'b', 'c')
('a', 'b', 'c')
>>> (1.0, 2.0, 3.0)
(1.0, 2.0, 3.0)
>>> (1 + 2j, 2 + 3j, 3 + 4j)
((1+2j), (2+3j), (3+4j))
```

## Sets

```python
>>> {1, 2, 3}
{1, 2, 3}
>>> {'a', 'b', 'c'}
{'a', 'b', 'c'}
>>> {1.0, 2.0, 3.0}
{1.0, 2.0, 3.0}
>>> {1 + 2j, 2 + 3j, 3 + 4j}
{(1+2j), (2+3j), (3+4j)}
```

## Dictionaries

```python
>>> {'a': 1, 'b': 2, 'c': 3}
{'a': 1, 'b': 2, 'c': 3}
>>> {'a': 'a', 'b': 'b', 'c': 'c'}
{'a': 'a', 'b': 'b', 'c': 'c'}
>>> {'a': 1.0, 'b': 2.0, 'c': 3.0}
{'a': 1.0, 'b': 2.0, 'c': 3.0}
>>> {'a': 1 + 2j, 'b': 2 + 3j, 'c': 3 + 4j}
{'a': (1+2j), 'b': (2+3j), 'c': (3+4j)}
```

## None

```python
>>> None
```

## Type

```python
>>> type(1)
<class 'int'>
>>> type(1.0)
<class 'float'>
>>> type(1 + 2j)
<class 'complex'>
>>> type('Hello World')
<class 'str'>
>>> type(True)
<class 'bool'>
>>> type([1, 2, 3])
<class 'list'>
>>> type((1, 2, 3))
<class 'tuple'>
>>> type({1, 2, 3})
<class 'set'>
>>> type({'a': 1, 'b': 2, 'c': 3})
<class 'dict'>
>>> type(None)
<class 'NoneType'>
```

## Type casting

```python
>>> int(1.0)
1
>>> int(1 + 2j)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: can't convert complex to int
>>> int('Hello World')
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
ValueError: invalid literal for int() with base 10: 'Hello World'
>>> int(True)
1
>>> int(False)
0
>>> int([1, 2, 3])
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: int() argument must be a string, a bytes-like object or a number, not 'list'
>>> int((1, 2, 3))
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: int() argument must be a string, a bytes-like object or a number, not 'tuple'
>>> int({1, 2, 3})
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: int() argument must be a string, a bytes-like object or a number, not 'set'
>>> int({'a': 1, 'b': 2, 'c': 3})
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
ValueError: invalid literal for int() with base 10: 'a'
>>> int(None)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: int() argument must be a string, a bytes-like object or a number, not 'NoneType'
>>> float(1)
1.0
>>> float(1 + 2j)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: can't convert complex to float
>>> float('Hello World')
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
ValueError: could not convert string to float: 'Hello World'
>>> float(True)
1.0
>>> float(False)
0.0
>>> float([1, 2, 3])
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: float() argument must be a string or a number, not 'list'
>>> float((1, 2, 3))
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: float() argument must be a string or a number, not 'tuple'
>>> float({1, 2, 3})
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: float() argument must be a string or a number, not 'set'

>>> float({'a': 1, 'b': 2, 'c': 3})
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
ValueError: could not convert string to float: 'a'
>>> float(None)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: float() argument must be a string or a number, not 'NoneType'
>>> complex(1)
(1+0j)
>>> complex(1.0)
(1+0j)
>>> complex(1 + 2j)
(1+2j)
>>> complex('Hello World')
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
ValueError: complex() arg is a malformed string
>>> complex(True)
(1+0j)
>>> complex(False)
0j
>>> complex([1, 2, 3])
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: complex() argument must be a string or a number, not 'list'
>>> complex((1, 2, 3))
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: complex() argument must be a string or a number, not 'tuple'
>>> complex({1, 2, 3})
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: complex() argument must be a string or a number, not 'set'
>>> complex({'a': 1, 'b': 2, 'c': 3})
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
ValueError: complex() arg is a malformed string
>>> complex(None)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: complex() argument must be a string or a number, not 'NoneType'
>>> str(1)
'1'
>>> str(1.0)
'1.0'
>>> str(1 + 2j)
'(1+2j)'
>>> str('Hello World')
'Hello World'
>>> str(True)
'True'
>>> str(False)
'False'
>>> str([1, 2, 3])
'[1, 2, 3]'
>>> str((1, 2, 3))
'(1, 2, 3)'
>>> str({1, 2, 3})
'{1, 2, 3}'
>>> str({'a': 1, 'b': 2, 'c': 3})
"{'a': 1, 'b': 2, 'c': 3}"
>>> str(None)
'None'
>>> bool(1)
True
>>> bool(1.0)
True
>>> bool(1 + 2j)
True
>>> bool('Hello World')
True
>>> bool(True)
True
>>> bool(False)
False
>>> bool([1, 2, 3])
True
>>> bool((1, 2, 3))
True
>>> bool({1, 2, 3})
True
>>> bool({'a': 1, 'b': 2, 'c': 3})
True
>>> bool(None)
False
>>> list(1)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: 'int' object is not iterable
>>> list(1.0)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: 'float' object is not iterable
>>> list(1 + 2j)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: 'complex' object is not iterable
>>> list('Hello World')
['H', 'e', 'l', 'l', 'o', ' ', 'W', 'o', 'r', 'l', 'd']
>>> list(True)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: 'bool' object is not iterable
>>> list(False)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: 'bool' object is not iterable
>>> list([1, 2, 3])
[1, 2, 3]
>>> list((1, 2, 3))
[1, 2, 3]
>>> list({1, 2, 3})
[1, 2, 3]
>>> list({'a': 1, 'b': 2, 'c': 3})
['a', 'b', 'c']
>>> list(None)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module> 
TypeError: 'NoneType' object is not iterable  
>>> tuple(1)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: 'int' object is not iterable
>>> tuple(1.0)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: 'float' object is not iterable
>>> tuple(1 + 2j)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: 'complex' object is not iterable
>>> tuple('Hello World')
('H', 'e', 'l', 'l', 'o', ' ', 'W', 'o', 'r', 'l', 'd')
>>> tuple(True)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: 'bool' object is not iterable
>>> tuple(False)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: 'bool' object is not iterable
>>> tuple([1, 2, 3])
(1, 2, 3)
>>> tuple((1, 2, 3))
(1, 2, 3)
>>> tuple({1, 2, 3})
(1, 2, 3)
>>> tuple({'a': 1, 'b': 2, 'c': 3})
('a', 'b', 'c')
>>> tuple(None)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: 'NoneType' object is not iterable
>>> set(1)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: 'int' object is not iterable
>>> set(1.0)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: 'float' object is not iterable
>>> set(1 + 2j)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: 'complex' object is not iterable
>>> set('Hello World')
{'H', 'l', 'W', 'o', 'r', 'e', ' ', 'd'}
>>> set(True)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: 'bool' object is not iterable
>>> set(False)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: 'bool' object is not iterable
>>> set([1, 2, 3])
{1, 2, 3}
>>> set((1, 2, 3))
{1, 2, 3}
>>> set({1, 2, 3})
{1, 2, 3}
>>> set({'a': 1, 'b': 2, 'c': 3})
{'a', 'b', 'c'}
>>> set(None)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: 'NoneType' object is not iterable
>>> dict(1)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: 'int' object is not iterable
>>> dict(1.0)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: 'float' object is not iterable
>>> dict(1 + 2j)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: 'complex' object is not iterable
>>> dict('Hello World')
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: 'str' object is not iterable
>>> dict(True)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: 'bool' object is not iterable
>>> dict(False)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: 'bool' object is not iterable
>>> dict([1, 2, 3])
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: cannot convert dictionary update sequence element #0 to a sequence
>>> dict((1, 2, 3))
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: cannot convert dictionary update sequence element #0 to a sequence
>>> dict({1, 2, 3})
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: cannot convert dictionary update sequence element #0 to a sequence
>>> dict({'a': 1, 'b': 2, 'c': 3})
{'a': 1, 'b': 2, 'c': 3}
>>> dict(None)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: 'NoneType' object is not iterable
```

## References

- [Python Data Types (w3schools.com)](https://www.w3schools.com/python/python_datatypes.asp)
- [Python Data Types (programiz.com)](https://www.programiz.com/python-programming/variables-datatypes)
- [Python Data Types (tutorialspoint.com)](https://www.tutorialspoint.com/python/python_variable_types.htm)
- [Python Data Types (geeksforgeeks.org)](https://www.geeksforgeeks.org/python-data-types/)
- [Python Data Types (w3resource.com)](https://www.w3resource.com/python/python-data-types.php)
- [Python Data Types (learnpython.org)](https://www.learnpython.org/en/Variables_and_Types)
- [Python Data Types (python-course.eu)](https://www.python-course.eu/python3_variables.php)

