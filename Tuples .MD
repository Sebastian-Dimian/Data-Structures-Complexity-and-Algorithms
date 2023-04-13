
![Markdown Logo](https://images.interestingengineering.com/1200x675/filters:format(webp)/images/coding_channels.jpg)

# How to use Tuples in Python 3
1. Tuples are declared with parenthesis … aka round brackets
2. () is an empty tuple
3. (50,) is a singleton tuple; the comma is required
4. Tuples are sliceable; therefore, indexable using square brackets

## Tuple example
```Python
tup = ('C', ' Java', 'Python')
empty_tup = ()
single_tup = ('Park',)

print(tup)
print(empty_tup)
print(single_tup)
```
## Tuple Operators
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
















