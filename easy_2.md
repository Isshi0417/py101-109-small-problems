# Easy 2

### Welcome Stranger

Create a function that takes 2 arguments, a list and a dictionary. The list will contain 2 or more elements that, when joined with spaces, will produce a person's name. The dictionary will contain two keys, `"title"` and `"occupation"`, and the appropriate values. Your function should return a greeting that uses the person's full name, and mentions the person's tutle.

```python
def greetings(l, d):
    # join list into ful name
    name = " ".join(l)
    # concatenate title and occupation
    job = d['title'] + " " + d["occupation"]
    return f'Hello, {name}! Nice to have a {job} around.'
```

### Greeting a user

Write a program that asks for user's name, then greets the user. If the user appends a `!` to their name, the computer will yell the greeting (print it using all uppercase).

```python
name = input("What's your name? ")

# if ! is in input
if '!' in name:
    # print message and capitalize name
    print(f'HELLO {name.upper()} WHY ARE WE YELLING?')
else:
    print(f'Hello {name}.')
```

### Multiplying Two Numbers

Create a function that takes two arguments, multiplies them together, and returns the result.

```python
def multiply(n1, n2):
    return n1 * n2
```

### Squaring an Argument

Using the `multiply` function from the "Multiplying Two Numbers" exercise, write a function that computes the square of its argument (the square is the result of multiplying a number by itself).

```python
def multiply(n1, n2):
    return n1 * n2

def square(n):
    # invoke multiply() with same numbers
    return multiply(n, n)
```

### Floating Point Arithmetic

Write a program that prompts the user for two positive numbers (floating-point), then prints the results of the following operations on those two numbers: addition, subtraction, product, quotient, floor quotient, remainder, and power. Do not worry about validating the input.

```python
# convert input to float
n1 = float(input('Enter the first number:\n'))
n2 = float(input('Enter the second number:\n'))

# print results
print(f'{n1} + {n2} = {n1 + n2}')
print(f'{n1} - {n2} = {n1 - n2}')
print(f'{n1} * {n2} = {n1 * n2}')
print(f'{n1} / {n2} = {n1 / n2}')
print(f'{n1} // {n2} = {n1 // n2}')
print(f'{n1} % {n2} = {n1 % n2}')
print(f'{n1} ** {n2} = {n1 ** n2}')
```

### The End is Near But Not Here

Write a function that returns the next to last word in the string argument.

Words are any sequence of non-blank characters.

You may assume that the input string will always contain at least two words.

```python
def penultimate(s):
    # split string into list
    l = s.split()
    # return the second last element from list
    return l[-2]
```

### Exclusive Or

The `or` operator returns a truthy value if either or both of its operands are truthy, a falsy value if both operands are falsy. The `and` operator returns a truthy value if both of its operands are truthy, and a falsy if either operand is falsy. This works great until you need only one of two conditions to be truthy, the so-called **exclusive or**, also known as **xor** (pronounced "ECKS-or").

In this exercise, you will write an `xor` function that takes two arguments, and returns `True` if exactly one of its arguments is truthy, `False` otherwise.

```python
def xor(a1, a2):
    if (a1 and not a2) or (not a1 and a2):
        return True
    return False
```

### Odd Lists

Write a function that returns a list that contains every other element of a list that is passed in as an argument. The values in the returned list should be those values that are in the 1st, 3rd, 5th, and so on element of the argument list.

```python
def oddities(full_list):
    # initialize empty list
    odd_list = []
    # each even index (odd position)
    for index in range(0, len(full_list), 2):
        # append to empty list
        odd_list.append(full_list[index])
    return odd_list
```

