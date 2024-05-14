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

