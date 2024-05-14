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

