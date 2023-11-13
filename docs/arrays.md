# Python Arrays

## Arrays

Arrays are used to store multiple values in one single variable:

```python
cars = ["Ford", "Volvo", "BMW"]
```

## What is an Array?

An array is a special variable, which can hold more than one value at a time.

If you have a list of items (a list of car names, for example), storing the cars in single variables could look like this:

```python
car1 = "Ford"
car2 = "Volvo"
car3 = "BMW"
```

However, what if you want to loop through the cars and find a specific one? And what if you had not 3 cars, but 300?

The solution is an array!

An array can hold many values under a single name, and you can access the values by referring to an index number.

## Access the Elements of an Array

You refer to an array element by referring to the index number.

```python
cars = ["Ford", "Volvo", "BMW"]

x = cars[0]

print(x)

'Ford'
```

## Modify the Value of the First Array Item

To modify the value of the first item in the array, refer to the index number:

```python
cars = ["Ford", "Volvo", "BMW"]

cars[0] = "Toyota"
```

## The `len()` Method

The `len()` method returns the number of elements in an array:

```python
cars = ["Ford", "Volvo", "BMW"]

x = len(cars)
```

## Looping Array Elements

You can use the `for in` loop to loop through all the elements of an array.

```python
cars = ["Ford", "Volvo", "BMW"]
for x in cars:
  print(x)
```

## Adding Array Elements

You can use the `append()` method to add an element to an array.

```python
cars = ["Ford", "Volvo", "BMW"]

cars.append("Honda")
```

## Removing Array Elements

You can use the `pop()` method to remove an element from the array.

```python
cars = ["Ford", "Volvo", "BMW"]

cars.pop(1)
```

You can also use the `remove()` method to remove an element from the array.

```python
cars = ["Ford", "Volvo", "BMW"]

cars.remove("Volvo")
```

## Array Methods

Python has a set of built-in methods that you can use on lists/arrays.

| Method | Description |
| --- | --- |
| `append()` | Adds an element at the end of the list |
| `clear()` | Removes all the elements from the list |
| `copy()` | Returns a copy of the list |
| `count()` | Returns the number of elements with the specified value |
| `extend()` | Add the elements of a list (or any iterable), to the end of the current list |
| `index()` | Returns the index of the first element with the specified value |
| `insert()` | Adds an element at the specified position |
| `pop()` | Removes the element at the specified position |
| `remove()` | Removes the item with the specified value |
| `reverse()` | Reverses the order of the list |
| `sort()` | Sorts the list |
