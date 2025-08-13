# 5.	Coding Standard Used in Industry:


### 1. Naming Conventions
- Use meaningful names for variables, functions, and classes.
- Variables → snake_case (e.g., total_amount).
- Functions → snake_case (e.g., calculate_total()).
- Classes → PascalCase (e.g., BankAccount).
- Example:
```python
python
CopyEdit
class BankAccount:
    def __init__(self, account_holder):
        self.account_holder = account_holder
        
```

### 2. Indentation & Spacing
- 4 spaces per indentation level (PEP8 standard in Python).
- Leave one blank line between functions.
- Space after commas, around operators (=, +, -).
- Example:
```python
python
CopyEdit
x = 10
y = 20
result = x + y
```

### 3. Commenting & Documentation
- Use # for single-line comments.
- Use docstrings (""" """) for functions, classes, and modules.
- Example:
```python
python
CopyEdit
def calculate_area(radius):
    """Calculate area of a circle given its radius."""
    return 3.14 * radius * radius
```    

### 4. Consistent File Structure
- Organize imports at the top.
- Keep constants in uppercase.
- Separate code logic, config, and data into different files.
- Example:
```python
python
CopyEdit
import math
PI = 3.14
```

### 5. Avoid Hardcoding
- Use variables, constants, or config files instead of magic numbers.
- Example:
```python
python
CopyEdit
TAX_RATE = 0.18
total_price = 1000
final_price = total_price + (total_price * TAX_RATE)
```

### 6. Error Handling
- Use try-except to handle runtime errors gracefully.
- Example:
```python
python
CopyEdit
try:
    num = int(input("Enter a number: "))
    print(10 / num)
except ValueError:
    print("Invalid input!")
except ZeroDivisionError:
    print("Cannot divide by zero!")
    
```

### 7. Testing & Code Reviews
- Test code before deployment.
- Use tools like pytest or unittest.
- Follow team review processes.

