# **Map & Filter In Python 3**

![Markdown Logo](https://blog-media.byjusfutureschool.com/bfs-blog/2022/08/03035002/Article-Image-945%C3%97498.jpg)

# Map Function

The idea of a map function is to apply a function to an iterable data.

Formatting:
map(function_name, sequence)

1. function_name: any function (built-in or selfmade) that returns a desired value of choice
2. sequence: any iterable data type


# Example
```Python
def square(num):
    ''' squares the given num argument '''
    return num ** 2
# end of square

array = list(range(1,11))
square_array = list(map(square, array))

print('Original Array:', array)
print('Array Squared:', square_array)
```

**Note:** One thing to note about the map function is that it doesn’t return a specific data type, but rather, an python iterable data. Therefore, after we apply the map function, we just execute a list function on it.

# Filter Function

The idea of the filter function is to filter out items from a data set that meets a certain condition.
Formatting:
filter(bool_returning_function, sequence)

```Python

def isOdd(x):
    ''' isOdd() returns True if x is odd.'''
    return x % 2 != 0

array = list(range(1,101))
odds = list(filter(isOdd, array))

print('Odd Numbers from 1 to 100:', odds)
```
The code show we can filter out variables that satisfies condition… aka the condition is True.

# Composition of Functions

Composition of Functions is the idea of using functions within a function call or apply one function to the result of another function. 






