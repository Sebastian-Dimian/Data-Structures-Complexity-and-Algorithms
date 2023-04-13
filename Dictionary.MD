# Dictionary in python 3

![Markdown Logo](https://images.pexels.com/photos/546819/pexels-photo-546819.jpeg?cs=srgb&dl=pexels-luis-gomes-546819.jpg&fm=jpg)

## Defining a Dictionary in Python 3

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
