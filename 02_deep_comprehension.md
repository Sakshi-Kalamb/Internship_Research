# 2.	Deep Comprehension: 

	Comprehensions: are a compact way to create new sequences (list, set, dictionary) from existing iterables.

##	Basic Syntax:

[expression for item in iterable if condition]

 a.	expression → what you want to store in the list  
 b.	item → variable that takes each value from the iterable (like a list, range, string, etc.)  
 c.	iterable → sequence to loop through  
 d.	condition (optional) → filters which items to include  
##	Types:
 a.	List Comprehension → Creates lists  
 b.	Set Comprehension → Creates sets (no duplicates)  
 c.	Dictionary Comprehension → Creates dictionaries (key–value pairs)  
 d.	Nested Comprehension → Comprehension inside another comprehension  
 e.	Conditional Expression in Comprehension →Condition inside comprehension  


## a.	List Comprehension:
```python
# Basic list creation 
numbers = [i for i in range(5)] 
print(numbers) # [0, 1, 2, 3, 4] 
# With condition 
evens = [i for i in range(10) if i % 2 == 0] 
print(evens) # [0, 2, 4, 6, 8] 
# With transformation 
squares = [i**2 for i in range(6)] 
print(squares) # [0, 1, 4, 9, 16, 25] 
```

## b.	Set Comprehension:
```python
# Removes duplicates automatically 
unique_nums = {i for i in [1, 2, 2, 3, 3, 4]} 
print(unique_nums) # {1, 2, 3, 4} 
```

## c.	Dictionary Comprehension:
```python
# Basic dictionary comprehension
squares_dict = {x: x**2 for x in range(5)}
print(squares_dict)  # {0: 0, 1: 1, 2: 4, 3: 9, 4: 16}

# With condition
even_squares_dict = {x: x**2 for x in range(10) if x % 2 == 0}
print(even_squares_dict)  # {0: 0, 2: 4, 4: 16, 6: 36, 8: 64}
```


## d.	Nested Comprehension:
```python
# Flatten a matrix
matrix = [[1, 2], [3, 4], [5, 6]]
flat = [num for row in matrix for num in row]
print(flat)  # [1, 2, 3, 4, 5, 6]

# Multiplication table
table = [f"{i}x{j}={i*j}" for i in range(1, 4) for j in range(1, 4)]
print(table)  
# ['1x1=1', '1x2=2', '1x3=3', '2x1=2', '2x2=4', '2x3=6', '3x1=3', '3x2=6', '3x3=9']
```


## e.	Conditional Expression in Comprehension:
```python
# Using if-else inside comprehension
status = ["even" if i % 2 == 0 else "odd" for i in range(6)]
print(status)  # ['even', 'odd', 'even', 'odd', 'even', 'odd']
```
