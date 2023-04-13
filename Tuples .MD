# Tuples in Python 3

![Markdown Logo](https://images.interestingengineering.com/1200x675/filters:format(webp)/images/coding_channels.jpg)

## _How to use Tuples in Python 3_
1. Tuples are declared with parenthesis … aka round brackets
2. () is an empty tuple
3. (50,) is a singleton tuple; the comma is required
4. Tuples are sliceable; therefore, indexable using square brackets

## _Tuple example_
```Python
tup = ('C', ' Java', 'Python')
empty_tup = ()
single_tup = ('Park',)

print(tup)
print(empty_tup)
print(single_tup)
```
## _Tuple Operators_
```Python
a = (1,2,3)
b = (4,5,6)
concat_result = a + b
print('a+b:', concat_result)


# Repetition: Repeating a list multiple times
c = ('Hi!',)
repet_result = c * 3
print('c*3', repet_result)

# Membership: Check if a value exists in a tuple
d = a + b + c
print('d:', d)
print('\'Hi!\' in d:', 'Hi!' in d)
print('7 in d:', 7 in d)
```
Tuple's have multiple functions like how they are also Iterable, Indexable, and Sliceable. 

## _Tuple Comprehension_

```Python
even_tup = tuple(i for i in range(1,101) if i % 2 == 0)

print(even_tup)
```
The parentheses were taken for a different functionality in python; therefore, we have to do comprehension like this. The general format is the exactly the same as list comprehension.

## _Packing and Unpacking_

```Python
var_1 = 2
var_2 = 3
var_3 = 5

prime = var_1, var_2, var_3

print('Packed prime values:', prime)

# Unpacking and Repacking
fib = (0, 1, 1, 2, 3, 5, 8)

fib_0, fib_1, fib_n = fib[0], fib[1], fib[2:]
print('fib_0:', fib_0)
print('fib_1:', fib_1)
print('fib_n:', fib_n)
```

__How it works:__

1. Packing collect multiple variable’s values and assign it to a single variable
2. Unpacking help us assign certain values from a tuple to different variables
3. This becomes very useful skill when combined with variable arguments for Function Definition and Function Calls

















