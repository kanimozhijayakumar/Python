Here are Python interview questions with examples:

1. **What is the difference between `is` and `==`?**  
   - `is`: Checks object identity.  
   - `==`: Checks value equality.  
   ```python
   a = [1, 2, 3]
   b = a
   c = [1, 2, 3]
   print(a is b)  # True
   print(a == c)  # True
   print(a is c)  # False
   ```

2. **Explain Python decorators.**  
   - A decorator modifies the behavior of a function or class.  
   ```python
   def decorator(func):
       def wrapper():
           print("Before function")
           func()
           print("After function")
       return wrapper
   
   @decorator
   def hello():
       print("Hello, World!")
   
   hello()
   ```

3. **What is the difference between a shallow copy and a deep copy?**  
   - Shallow copy: Copies the reference, not the actual objects.  
   - Deep copy: Creates a new copy of the objects.  
   ```python
   import copy
   original = [[1, 2], [3, 4]]
   shallow = copy.copy(original)
   deep = copy.deepcopy(original)
   original[0][0] = 99
   print(shallow)  # [[99, 2], [3, 4]]
   print(deep)     # [[1, 2], [3, 4]]
   ```

4. **How does Python handle exceptions?**  
   - Using `try`, `except`, and optionally `finally`.  
   ```python
   try:
       x = 10 / 0
   except ZeroDivisionError as e:
       print("Cannot divide by zero:", e)
   finally:
       print("Execution completed.")
   ```

5. **What are Python’s data types?**  
   - Examples: `int`, `float`, `str`, `list`, `tuple`, `set`, `dict`.  
   ```python
   my_list = [1, 2, 3]       # List
   my_tuple = (1, 2, 3)      # Tuple
   my_set = {1, 2, 3}        # Set
   my_dict = {'a': 1, 'b': 2} # Dictionary
   ```
