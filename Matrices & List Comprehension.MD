# __Matrices & List Comprehension__
![Markdown Logo](https://woz-u.com/wp-content/uploads/2022/06/Evolution-of-Coding-scaled.jpg)

## **What is Matrix**
matrix is a representations of numbers, symbols, or expressions in a 2-Dimensional Array. With Python, we can start to create a data structure that has values in rows and columns, much like a table, by utilizing a list within a list.

## **Example**
```Python
matrix_A = [
    [1, 2, 3, 4],
    [5, 6, 7, 8]
]
```
# Rules
1.  In Python 3, there is no data structure called a "Matrix". Therefore we have to follow the rules:
    1. All rows must have the same number of values
    2. All columns must have the same number of values
    3. All items in the 2D List must have the same data types
    4. Since indexing always starts at 0 ... row 1 is technically located at matrix_A[0]
    
# **List Comprehension**
List Comprehension is a concise method to create list in Python 3.

This technique is commonly used when:

1.  The list is a result of some operations applied to all its items
2.  It is a made from another sequence/iterable data
3.  The list is member of another list/sequence/iterable data that satisfies a certain condition

## **Example code**
```Python
squares = [i**2 for i in range(10)]

print('Our new result: %s' % squares)
```

# Explanation
List comprehension consists of:

A Square Bracket containing an expression that describes the list
One or more For clause to explain its members
Then a zero or more if clauses depending on the complexity of the list
Examine: [i**2 for i in range(10)]

1.   i**2 for i in range(10) --> is the expression that describe the list
2.   i**2 describes each item in the list
3.   i is taken from the for clause
4.   for i in range(10) describes where i comes from

**Note:** With list comprehension, the order of your for clauses matter!




















