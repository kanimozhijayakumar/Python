
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

6. **What are Python’s key features?**  
   - High-level, interpreted, dynamically typed, object-oriented, extensive libraries, and cross-platform.  
   ```python
   # Dynamic typing
   x = 10
   x = "Python"  # No need to declare the type explicitly
   print(x)  # Output: Python
   ```

7. **Explain the use of `self` in Python classes.**  
   - `self` refers to the current instance of the class and is used to access instance variables and methods.  
   ```python
   class MyClass:
       def __init__(self, name):
           self.name = name
       def greet(self):
           return f"Hello, {self.name}!"

   obj = MyClass("Alice")
   print(obj.greet())  # Output: Hello, Alice!
   ```

8. **What is Python's Global Interpreter Lock (GIL)?**  
   - GIL ensures that only one thread executes Python bytecode at a time, limiting multi-threaded performance in CPU-bound tasks.  
   ```python
   import threading
   count = 0
   def increment():
       global count
       for _ in range(1000000):
           count += 1
   
   thread1 = threading.Thread(target=increment)
   thread2 = threading.Thread(target=increment)
   thread1.start()
   thread2.start()
   thread1.join()
   thread2.join()
   print(count)  # Output may not be 2000000 due to GIL
   ```

9. **What are Python decorators?**  
   (Example already provided in the earlier response.)

10. **How is memory managed in Python?**  
   - Python uses automatic memory management with reference counting and garbage collection.  
   ```python
   a = [1, 2, 3]
   b = a  # Reference count for the list increases
   del a  # Reference count decreases
   # When no references are left, the memory is freed
   ```
