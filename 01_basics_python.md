
# Python Basics with Examples


## 1. Variables
- Store data values.
 - Dynamic typing (no need to declare type explicitly).
   
```python
x = 10  # integer
name = "Sakshi"  # string
print(x, name)
```

## 2. Data Types
 - Different types of data Python can handle (int, float, str, bool, list, tuple, dict).
 - Helps in performing type-specific operations.
```python
age = 20          # int
height = 5.2      # float
is_student = True # boolean
print(type(age), type(height), type(is_student))
```

## 3. Operators
 - Symbols to perform operations like +, -, *, /.
 - Include arithmetic, comparison, logical operators.
```python
a = 5
b = 3
print(a + b)   # 8
print(a > b)   # True
print(a == b)  # False
```

## 4. Conditional Statements
 - Execute code based on conditions using if, elif, else.
 - Control the flow of the program.
   
```python
num = 10
if num > 0:
    print("Positive")
elif num == 0:
    print("Zero")
else:
    print("Negative")
```

## 5. Loops
 - Repeat a block of code multiple times.
 - Types: for loop, while loop.
 For loop example:
```python
for i in range(5):
    print(i)
# While loop example:
count = 0
while count < 3:
    print("Hello")
    count += 1
```

## 6. Functions
 - Reusable blocks of code to perform a task.
 - Defined using def keyword.
   
```python
def greet(name):
    return f"Hello, {name}!"
print(greet("Sakshu"))
```

## 7. Lists
 - Ordered collection of items, mutable (can change).
 - Supports indexing, slicing, appending, removing.
```python
fruits = ["apple", "banana", "cherry"]
fruits.append("orange")
print(fruits)
print(fruits[1])  # banana
```

## 8. Tuples
- Ordered collection of items, immutable (cannot change).
 - Useful for fixed data.
```python
coordinates = (10, 20)
print(coordinates)
print(coordinates[0])  # 10
```

## 9. Dictionaries
 - Key-value pairs to store data.
 - Keys are unique; values can be any type.
```python
student = {"name": "Sakshi", "age": 20}
print(student["name"])
student["age"] = 21  # update value
print(student)
```

## 10. Strings
 - Sequence of characters.
 - Supports indexing, slicing, concatenation.
```python
text = "Hello Python"
print(text[0])     # H
print(text[0:5])   # Hello
print(text + "!!") # Hello Python!!
```

## 11. Input & Output
 - Take input from user using input().
 - Display output using print().
```python
user_name = input("Enter your name: ")
print("Welcome,", user_name)
```

## 12. Comments
 -  Notes in code ignored by Python.
 -  Single-line using #, multi-line using ''' '''.
   
```python
# This is a single-line comment
'''
This is
a multi-line comment
'''

```
