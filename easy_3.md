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

### Bannerizer

Write a function that takes a short line of text and prints it within a box.

```python
def print_in_box(string):
    width = len(string)
    box_line = '-'
    box = f'''
    +{box_line * (width + 2)}+
    | {' ' * width} |
    | {string} |
    | {' ' * width} |
    +{box_line * (width + 2)}+
    '''
    print(box)
```

### Strings Strings

Write a function that takes one argument, a positive integer, and returns a string of alternating `'1'`s and `'0'`s, always starting with a `'1'`. The length of the string should match the given integer.

```python
def stringy(n):
    string = ''
    # foe each number in n
    for i in range(n):
        # if number is odd
        if i % 2 == 1:
            string += '0'
        else:
            string += '1'
    return string
```

### Right Triangles

Write a function that takes a positive integer, `n`, as an argument and prints a right triangle whose sides each have `n` stars. The hypotenuse of the triangle (diagonal side in the images below) should have one end at the lower-left of the triangle, and the other end at the upper-right.

```python
def triangle(n):
    for i in range(n):
        print(f'{' ' * (n - i)}{'*' * i}')
```

### Madlibs

Madlibs is a simple game where you create a story template with "blanks" for words. You, or another player, then construct a list of words and place them into the story, creating an often silly or funny story as a result.

Create a simple madlib program that prompts for a noun, a verb, an adverb, and an adjective, and injects them into a story that you can create.

```python
noun = input('Enter a noun: ')
verb = input('Enter a verb: ')
adjective = input('Enter an adjective: ')
adverb = input('Enter an adverb: ')

print(f'Do you walk your {adjective} {noun} {adverb}? That\'s hilarious!')
print(f'The {adjective} {noun} {verb}s {adjective} over the lazy dog.')
print(f'The {noun} {adjective} {verb}s up to Joe\'s blue turtle.')
```

