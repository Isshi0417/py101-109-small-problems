# Easy 3

### Repeat Yourself

Write a function that takes two arguments, a string and a positive integer, then prints the string as many times as the integer indicates.

```python
def repeat(s, n):
    for i in range(n):
        print(s)
```

### ddaaiillyy ddoouubbllee

Write a function that takes a string argument and returns a new string that contains the value of the original string with all consecutive duplicate characters collapsed into a single character.

```python
def crunch(string):
    crunched = ''
    # for each letter in string
    for index in range(len(string)):
        # if letter is not in crunched or the letter before is not the same
        if string[index] not in crunched or string[index - 1] != string[index]:
            crunched += string[index]
    return crunched
```

