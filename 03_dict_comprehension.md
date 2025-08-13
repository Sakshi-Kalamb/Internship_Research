# Dict Comprehension


It creates a dictionary (key–value pairs) in a single line using a loop (and optionally conditions).

## 1. Basic Syntax

### {key_expr: value_expr for item in iterable if condition}  
- key_expr → expression for the dictionary key

- value_expr → expression for the dictionary value

- iterable → any iterable (list, range, string, etc.)

- condition (optional) → filter items

### Examples
- Create dictionary from a list

```python
numbers = [1, 2, 3, 4]
squares = {num: num**2 for num in numbers}
print(squares)
Output:


{1: 1, 2: 4, 3: 9, 4: 16}

```
- Filter items while creating dictionary
```python
numbers = [1, 2, 3, 4, 5]
even_squares = {num: num**2 for num in numbers if num % 2 == 0}
print(even_squares)
Output:


{2: 4, 4: 16}
```

- Swap keys and values
```python
data = {"a": 1, "b": 2, "c": 3}
swapped = {value: key for key, value in data.items()}
print(swapped)
Output:

{1: 'a', 2: 'b', 3: 'c'}
```

