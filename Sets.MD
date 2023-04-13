# Sets in Python 3
________________________________________

![Markdown Logo](https://www.simplilearn.com/ice9/free_resources_article_thumb/python_sets_and_dictionaries.jpg)

## __What is a set__

A set is an unordered collection with no duplicate elements in Python 3. Set is a mathematical way to describe collection of different unique objects.

__Example:__
```Python
example_set1 = {1, 2, 3}
example_set2 = {'h','e','l','l','o'}

print('example_set1:', example_set1)
print('example_set2:', example_set2) # Notice there is only 1 'l'; Also notice the order of the values outputted
print('--')

singleton_set = {7}
empty_set = set() # this is because {} is reversed for a different feature in python 3.

print('Singleton:', singleton_set)
print('Empty Set:', empty_set)
```

## Basic Membership Operators
Membership is one of the key operations with set because
1.    A set has no duplicates
2.    A set’s membership operation is one of the fastest operations compared to strings, lists, or tuples this will be covered more when we look at the concept of: complexity
3.    By using membership operator, we can be certain a target exists or does not exist in our data

## Accessing values in a Set
- Due to its unordered nature of a set, there is no concept of indexing or slicing with a set.
- Set is however iterable.

__Example:__
```Python
example_set = {2,3,5,7,11,13}

for v in example_set:
    print('Values of example_set:', v)
```

## Sets are also Mutable!
Adding and removing values
  1.    Sets are mutable; therefore, we can add and remove values
  2.    There are also methods much lists that can affect the original sets as well


## Powering Up Sets: Set Operators

Much like its mathematical counterpart, sets in Python 3 can utilize its vast operators to help us do complex calculations. Most of these operators will have a method counterpart because sets are mutable. Note: We will be showcasing these operators with set of strings to make our lives easier, but this can be easily done with any kinds of sets


1. __Union:__ The joining/combining of two sets.
2. __Intersection:__ Members/Items that only exists in both sets.
3. __Difference:__ Members/items that only exists in the first set and not the second set.
4. __Symmetric Difference:__ Members/items that exists one or the other set, but not both sets
5. __Proper Subset:__ This is a boolean operator. A is proper subset of B if all members of A is found in B, but A cannot be exactly the same as B
6. __Subset:__ This is a boolean operator. A is a Proper Subset of B if A < B is True, but A can equal to B unlike a proper subset
7. __Proper Superset:__ This is a boolean operator. A is a proper superset of B if A has all the values of B and more, but they are not equal to each other
8. __Superset:__ This is a boolean operator. A is a superset of B if A > B or A == B


## Disjoint: A Set Behaviour Property
Two set are consided disjointed when two sets share no common value.

- Let A and B both represent a set.
- If A & B is empty, then set A and B are considered disjointed.
- To check this in python there is a method called: isdisjoint()

__Example__
```Python

set1 = {1,2,3,4}
set2 = {5,6,7}
set3 = {1,2,3,4,5}

print('set1 intersect set2:', set1 & set2) # Output is an empty set
print('set1 intersect set3:', set1 & set3) # Output is an non-empty set
print('--')
print('set 1 disjoint set 2 check:', set1.isdisjoint(set2)) # Therefore .isdisjoint() evaluates to True
print('set 1 disjoint set 3 check:', set2.isdisjoint(set3))
```

## Set Comprehension

```Python
def isPalindrome(x):
    ''' isPalindrome() returns True if string X is a palindrome '''
    return x == x[::-1]

nums = list(range(1,10000))
palindromic_set = {num for num in nums if isPalindrome(str(num))}

print('Palindromic Numbers Set from 1 to 10000:')
print(palindromic_set)
```
Much like list comprehension, sets support comprehension as well.


## __Important Notes to take away:__
1. Sets aren’t sliceable nor indexable
2. Sets cannot have sets inside them
3. Sets do not have order; nor order of insertion
4. Sets cannot guarantee that their values will be in order
5. Sets do not record a value’s position













