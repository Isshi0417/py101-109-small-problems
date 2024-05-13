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
# for each number after 1 added by 2
for i in range(1, 100, 2):
    print(i)
```

### Even Numbers

Print all even numbers from `1` to `99`, inclusive, with each number on a separate line.

```python
# for each number between 1 and 99
for i in range(1, 100):
    # if remainder is 0
    if i % 2 == 0:
        print(i)
```

Can you solve the problem over just the even numbers?

```python
# for each number after 2 added by 2
for i in range(2, 100, 2):
    print(i)
```

### How big is the room?

Build a program that asks the user to enter the length and width of a  room, in meters, then prints the room's area in both square meters and  square feet.

*Note*: 1 square meter == 10.7639 square feet

```python
# ask for user input
l = float(input('Enter the length of the room in meters: '))
w = float(input('Enter the width of the room in meters: '))

# calculate area
area = l * w

# print result
print(f'Area of the room (meters): {area} square meters.')
print(f'Area of the room (sq. ft): {area * 10.7639} square feet.')
```

### Tip Calculator

Create a simple tip calculator. The program should prompt for a bill amount and a tip rate. The program must compute the tip, then print both the tip and the total amount of the bill. You can ignore input validation and assume that the user will enter valid numbers.

```python
# ask for input
bill = float(input('What is the bill? '))
tip_percentage = float(input('What is the tip percentage? '))

# calculate tip
tip = bill * (tip_percentage / 100)
total = bill + tip

# print results
print(f'The tip is ${tip:.2f}')
print(f'The total is ${total:.2f}')
```

