# List Comprehension

- Shorter, cleaner way to create lists in Python using a single line.
- More readable and slightly faster than normal loops.

## Syntax
[expression for item in iterable if condition]


- expression → what you want to store in the list
-	item → variable that takes each value from the iterable (like a list, range, string, etc.)  
-	iterable → sequence to loop through  
-	condition (optional) → filters which items to include  




## Examples



a.	Normal loop:
```python
numbers = []
for i in range(5):
    numbers.append(i * 2)
print(numbers)  # [0, 2, 4, 6, 8]
```

b.	List comprehension:
```python
numbers = [i * 2 for i in range(5)]
print(numbers)  # [0, 2, 4, 6, 8]
```

c.	With Condition:
```python
even_numbers = [i for i in range(10) if i % 2 == 0]
print(even_numbers)  # [0, 2, 4, 6, 8]
```

d.	Nested List Comprehension:
```python
matrix = [[j for j in range(3)] for i in range(3)]
print(matrix)
# [[0, 1, 2], [0, 1, 2], [0, 1, 2]]
```


