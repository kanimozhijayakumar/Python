

---

## File Processing in Python

File processing in Python involves handling files for various operations such as creating, reading, writing, updating, and deleting content. Python provides a simple and efficient way to work with files using built-in functions and context management.

### Key Features of File Processing:
1. **File Modes**: Determines how the file is accessed. Common modes include:
   - `'r'` - Read mode (default).
   - `'w'` - Write mode (overwrites existing content).
   - `'a'` - Append mode (adds content to the end of the file).
   - `'b'` - Binary mode for non-text files.

2. **Opening Files**: Use the `open()` function:
   ```python
   file = open("example.txt", "r")  # Opens a file in read mode
   ```

3. **Reading Files**:
   - `file.read()` - Reads the entire file.
   - `file.readline()` - Reads one line at a time.
   - `file.readlines()` - Reads all lines into a list.
   ```python
   with open("example.txt", "r") as file:
       content = file.read()
       print(content)
   ```

4. **Writing Files**:
   - `file.write("text")` - Writes content to a file.
   - `file.writelines()` - Writes a list of strings.
   ```python
   with open("example.txt", "w") as file:
       file.write("Hello, Python!")
   ```

5. **Appending to Files**:
   ```python
   with open("example.txt", "a") as file:
       file.write("\nAdding more content.")
   ```

6. **Closing Files**:
   - Use `file.close()` to release resources.
   - Using `with open()` automatically handles closing.

7. **Sorting File Content**:
   To sort data in a file:
   ```python
   with open("data.txt", "r") as file:
       lines = file.readlines()

   sorted_lines = sorted(lines)

   with open("data.txt", "w") as file:
       file.writelines(sorted_lines)
   ```

### Benefits of File Processing in Python:
- Easy-to-use syntax for handling files.
- Support for text and binary files.
- Built-in error handling with `try-except` and `with` statement.

### Example: Reading and Writing a File
```python
# Writing to a file
with open("example.txt", "w") as file:
    file.write("Welcome to Python file processing!")

# Reading the file
with open("example.txt", "r") as file:
    content = file.read()
    print(content)
```

---
