# Dictionary in python 3

![Markdown Logo](https://images.pexels.com/photos/546819/pexels-photo-546819.jpeg?cs=srgb&dl=pexels-luis-gomes-546819.jpg&fm=jpg)

## Defining a Dictionary 

Dictionaries also use {} like sets; however, their individual item format is very different. Each item in a dictionary be a pair of key: value.

__Example:__
```Python
sammy = {
    'username': 'sammy',
    'online': True,
    'followers': 42
}

# There are 3 items: each with their unique addresses and value
# Accessing
print('Sammy dict:', sammy)
print('Username:', sammy['username'])
print('Online Status:', sammy['online'])
print('Follower Count:', sammy['followers'])
```
## Dictionary Properties
Each item in a dictionary is a key, value pair.
1. __Keys:__ Keys are unique address for a dictionary value’s location
2. __Key Properties:__
- Must be immutable (strings, numbers, tuples, frozenset)
- Unique; therefore, two same key values cannot exist in a single dictionary
- NEWEST CREATED ITEM with a duplicate KEY superceeds the previous declaration
3. __Values:__ Values of a dictionary within a key can be any data type.
4. __Updating a Dictionary:__ 
- We can modify existing values by referencing the key
- We can add new values to a dictionary by creating a new key
- We can overwrite a value at an existing key by referencing and recreating the value for it


## Deletion with Dictionary
1. We can delete a key hence deleting the value connected to the key
2. We can empty out the entire dictionary
3. We can delete the dictionary (uncommonly used)
 __Example:__
 ```Python
 sammy = {
    'username': 'sammy',
    'online': True,
    'followers': 42
}

del sammy['followers'] # del is a keyword used to help us to execute a removal
print('followers key deleted:', sammy)

sammy.clear() # {} is considered an empty dict
print('emptying out a dictionary', sammy)
print('--\n\n')

del sammy
print('Deleting sammy, should create an error when referenced again', sammy)
```
## Useful tips
1. __Memberships:__ We can use the in and not in operators to check if a key exists in a dictionary
2. __Built-in Functions with Dictionary:__ You are able to use built-in functions like len, max, min, str, and list with dictionary


## Dictionary Methods 

_Let A and B be a dictionary_

- A.keys() –> Returns a sequence of keys/addresses in A
- A.values() –> Returns a sequence of item values in A
- A.items() –> Returns a sequence of key,item pairs in A
- A.get(address) –> Returns the item value at address
- A.update(B) –> Extends A with the dictionary of key,value pairs of B
 __Example Code:__
```Python 
# Dictionary Method Examples

sammy = {
    'username': 'sammy',
    'online': True,
    'followers': 42
}

sammy_hidden = {
    'pwd' : 'qwerty',
    'location' : 'Toronto, Ontario'
}

# printing all the keys of a dict
print('Sammy Dict Keys:', sammy.keys()) # notice how it prints

sammy_keys = list(sammy.keys()) # we can listify the .keys() returned
print('List of sammy_keys', sammy_keys)
print('--')

# printing all the values of a dict
print('Sammy Dict Values:', sammy.values())
print('Sammy Dict Values as a list:', list(sammy.values()))
print('--')

# printing key, value pair of a dict
print('Sammy Dict key, value pairs:', sammy.items())
print('Sammy Dict key, value pairs as a list:', list(sammy.items()))
print('--')

# getting a value from a dict
print('Sammy followers value:', sammy.get('followers'))
print('Same as:', sammy['followers'])
print('--')

# updating / extending a dictionary
sammy.update(sammy_hidden)

print('Sammy extended with its hidden values:', sammy)
```

## Iterating a Dictionary
Iterating can be very helpful when coding, here are three iteration methods
1. iterating the keys
2. iterating the values
3. iterating the key, value pairs by unpacking

__Example code:__
```Python
# Iteration Example 1: Keys
sammy = {
    'username': 'sammy',
    'online': True,
    'followers': 42
}

for k in sammy.keys():
    print('Current key:', k)
print('--\n')

# Iteration Example 2: Values

for v in sammy.values():
    print('Current value:', v)
print('--\n')

# Iteration Example 3: Key, Value Pair

for k, v in sammy.items():
    print('Current Key:', k)
    print('Current Value:', v)
    print()
```
## Dictionary Comprehension

Using __dict() Constrcutor__ We can turn other data types to dictionaries. Also similar to lists, tuples, and sets, dictionaries also support comprehension.
_Note: We must specify where the keys are and where the values._
__Example code:__
```Python
example_data = [
    ('one', 3),
    ('two', 3),
    ('three', 5)
]

data_dict = dict(example_data)
print('data_dict:', data_dict)
print('--')

# Dictionary Comprehension
# Goal: Take string numerals and assign them with their integer square
# - keys : string numerals
# - values: integer squares

example_data2 = ['1', '2', '3', '4', '5']

data2_dict = {x : int(x)**2 for x in example_data2}

print('data2_dict:', data2_dict)
```



    
    
    
    
    
    
    
    
    
    
    







