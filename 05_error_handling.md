# 3.	Error Handling:

- Error handling is a way to manage unexpected problems during program execution so that the program does not crash.
- In Python, we mainly use try-except to catch and handle exceptions.

## Basic Syntax:

try:  
    # Code that may cause an error  
except:  
    # Code to run if error happens  

## Types:

a.	Try-Except: 
- Used to catch and handle exceptions
- Prevents program from crashing.
- Example:
```python
try: 
x = 10 / 0 
except ZeroDivisionError: 
print("Error: Division by zero occurred!") 
# Output: 
# Error: Division by zero occurred! 
```

b.	Try-Except-Else: 
- The else block runs only if no exception occurs.
- Helps separate error-handling code from normal execution code.

- Example:
```python
try: 
num = int("5") 
except ValueError: 
print("Invalid conversion!") 
else: 
print("Conversion successful:", num) 
# Output: 
# Conversion successful: 5 
```


c.	Try-Except-Finally: 
- finally block always executes, no matter what happens.
- Used for cleanup tasks (e.g., closing files, releasing resources).
- Example:
```python
try: 
file = open("test.txt", "w") 
file.write("Hello") 
except IOError: 
print("File error occurred!") 
finally: 
file.close() 
print("File closed successfully.") 
# Output: 
# File closed successfully.
```

d.	Raise : 
- Use raise to manually trigger an exception.
- Useful for enforcing rules or validation.

- Example: 
```python
try: 
age = -5 
if age < 0: 
raise ValueError("Age cannot be negative") 
except ValueError as e: 
print("Error:", e) 
# Output: 
# Error: Age cannot be negative 
```

e.	Assert:
- If the condition is False, it raises an AssertionError.
- Helps catch bugs early by validating assumptions in the code.
- Example:
```python
x = 10
y = 0
# Assert that y is not zero before division
assert y != 0, "Division by zero error!"

print(x / y)
# AssertionError: Division by zero error!
```
