# Small Problems: Easy 1

### Isn't it Odd?

Write a function that takes one integer argument and returns `True` when the number's absolute value is odd, False otherwise.

```python
def is_odd(n):
    return n % 2 == 1
    
print(is_odd(7))    # True
print(is_odd(10))   # False
print(is_odd(5))    # True
```

### Odd Numbers

Print all odd numbers from `1` to `99`, inclusive, with each number on a separate line.

```python
# for each number between 1 and 99
for i in range(1, 100):
    # if remainder is 1
    if i % 2 == 1:
        print(i)
```

Can you solve the problem by iterating over just the odd numbers?

```python
# for each number after one added by 2
for i in range(1, 100, 2):
    print(i)
```



