
### 1. **Variables**
Variables are used to store data that can be used later in the program. A variable is created when you assign a value to it.

Example:
```python
x = 10
name = "John"
```
Here, `x` stores the integer `10` and `name` stores the string `"John"`.

### 2. **Data Types**
Python supports various data types:
- **int**: Integer numbers, like `5`, `-2`, `100`.
- **float**: Decimal numbers, like `3.14`, `-0.1`, `2.0`.
- **str**: String (text) data, like `"Hello"`, `"Python"`.
- **bool**: Boolean values, either `True` or `False`.

Example:
```python
x = 10      # int
y = 3.14    # float
z = "Python" # str
is_active = True  # bool
```

### 3. **Operators**
Operators are used to perform operations on variables and values.
- **Arithmetic Operators**: `+`, `-`, `*`, `/`, `%` (modulus), `**` (exponentiation), `//` (floor division).
  Example:
  ```python
  x = 10
  y = 5
  sum = x + y   # 15
  division = x / y  # 2.0
  ```
- **Comparison Operators**: `==`, `!=`, `>`, `<`, `>=`, `<=`.
  Example:
  ```python
  x == y  # False
  x > y   # True
  ```
- **Logical Operators**: `and`, `or`, `not`.
  Example:
  ```python
  x = 10
  y = 5
  result = (x > y) and (y > 0)  # True
  ```

### 4. **Control Flow**
Control flow helps you direct the program's execution.
- **if-else**: Used for decision-making based on conditions.
  Example:
  ```python
  x = 10
  if x > 5:
      print("Greater than 5")
  else:
      print("Less than or equal to 5")
  ```
- **for loop**: Iterates over a sequence (like a list or range).
  Example:
  ```python
  for i in range(5):  # Loops from 0 to 4
      print(i)
  ```
- **while loop**: Repeats as long as a condition is true.
  Example:
  ```python
  count = 0
  while count < 5:
      print(count)
      count += 1
  ```

### 5. **Functions**
Functions are blocks of reusable code that perform specific tasks. You define a function using the `def` keyword.
Example:
```python
def greet(name):
    print(f"Hello, {name}!")

greet("Alice")  # Output: Hello, Alice!
```

### 6. **Lists**
A list is an ordered collection of items, which can be of any data type. Lists are mutable, meaning you can change their content.
Example:
```python
my_list = [1, 2, 3, "Hello", 3.14]
print(my_list[0])  # Output: 1
```

### 7. **Tuples**
A tuple is similar to a list, but it is immutable (its contents cannot be changed). Tuples are defined using parentheses `()`.
Example:
```python
my_tuple = (1, 2, 3, "Hello")
print(my_tuple[1])  # Output: 2
```

### 8. **Dictionaries**
A dictionary stores data in key-value pairs. Keys must be unique, and values can be any data type.
Example:
```python
my_dict = {"name": "John", "age": 25}
print(my_dict["name"])  # Output: John
```

### 9. **Classes and Objects**
Python supports object-oriented programming (OOP), allowing you to create classes and instantiate objects. A class defines the blueprint, and an object is an instance of that class.

Example:
```python
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age
        
person1 = Person("Alice", 30)
print(person1.name)  # Output: Alice
```

### 10. **Modules**
Modules are pre-written Python code that you can import and use. They provide functions and classes to perform specific tasks (e.g., math operations, file handling).

Example:
```python
import math
print(math.sqrt(16))  # Output: 4.0
```

