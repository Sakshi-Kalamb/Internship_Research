# 4.	File Handling:

- File handling allows you to store data permanently in files and retrieve it later.
- Useful for saving logs, storing user input, reading configurations, etc.
## Basic Steps:
a.	Open the file (open()) → Specify file name & mode.  
b.	Perform Operations → Read, Write, or Append.  
c.	Close the file (close()), unless using a with block.  
## File Modes
- "r" → Read (default)( File must exist)  
- "w" → Write (Creates file or overwrites if exists.)  
- "a" → Append (Creates file if not exists, adds at end)
- "x" → Create (Fails if file already exists)
- "rb", "wb", "ab" → Binary modes (images, videos, etc.)

##	Important Functions
- .read() → Reads whole file.
- .readline() → Reads one line at a time.
- .readlines() → Reads all lines into a list.
- .write() → Writes string data.
- .writelines() → Writes list of strings.

## Best Practice
Use with open(...) as file: → Automatically closes file.  
Handle exceptions using try-except.  
##	Example:
-  Writing to a file
```python
file = open("example.txt", "w")
file.write("Hello, this is the first line.\n")
file.write("This is the second line.")
file.close()
print("✅ Data written to file.")

#output
✅ Data written to file.
```


- Reading the file
```python
file = open("example.txt", "r")
content = file.read()
file.close()
print("\n📂 Reading file content:")
print(content)

# output 
📂 Reading file content:
Hello, this is the first line.
This is the second line.
```



-  Appending to the file
```python
file = open("example.txt", "a")
file.write("\nThis is an appended line.")
file.close()
print("\n✅ Data appended to file.")

# output 
📂 Reading file content:
Hello, this is the first line.
This is the second line.
```


-  Reading again to see updated content
```python
file = open("example.txt", "r")
updated_content = file.read()
file.close()
print("\n📂 Updated file content:")
print(updated_content)


# output 
📂 Updated file content:
Hello, this is the first line.
This is the second line.
This is an appended line.
"""
```













