# pythonbasics


### Basics
- **Comments**: `# This is a comment`
- **Variables**: `x = 5`
- **Data Types**: 
  - Integers: `x = 5`
  - Floating-point: `y = 5.0`
  - Strings: `name = "John"`
  - Boolean: `is_adult = True`
- **Type Conversion**: `int("5")`, `float("5")`, `str(5)`

### Operators
- **Arithmetic**: `+`, `-`, `*`, `/`, `%` (modulus), `**` (exponent), `//` (floor division)
- **Comparison**: `==`, `!=`, `<`, `>`, `<=`, `>=`
- **Logical**: `and`, `or`, `not`

### Control Structures
- **If Statement**:
  ```python
  if condition:
      # do something
  elif another_condition:
      # do something else
  else:
      # do another thing
  ```
- **Loops**:
  - For Loop:
    ```python
    for item in iterable:
        # do something with item
    ```
  - While Loop:
    ```python
    while condition:
        # do something
    ```

### Collections
- **List**: `my_list = [1, 2, 3]`
  - Indexing: `my_list[0]` (first item)
  - Slicing: `my_list[1:3]` (second to third item)
  - Append: `my_list.append(4)`
  - Remove: `my_list.remove(1)`
- **Tuple**: `my_tuple = (1, 2, 3)`
- **Set**: `my_set = {1, 2, 3}`
- **Dictionary**: `my_dict = {'key': 'value'}`
  - Access: `my_dict['key']`
  - Add/Update: `my_dict['new_key'] = 'new_value'`
  - Delete: `del my_dict['key']`

### Functions
```python
def my_function(param1, param2):
    # do something
    return result
```

### Classes
```python
class MyClass:
    def __init__(self, param1):
        self.param1 = param1

    def my_method(self):
        # do something
```

### Modules
- **Importing**: `import math`, `from math import sqrt`, `import math as m`

### File I/O
- **Reading a file**:
  ```python
  with open('file.txt', 'r') as f:
      content = f.read()
  ```
- **Writing to a file**:
  ```python
  with open('file.txt', 'w') as f:
      f.write('Hello, World!')
  ```

### Exceptions
```python
try:
    # try to do something
except ExceptionType:
    # handle exception
finally:
    # always do this
```

### Advanced Collections

#### Lists (More Details)
- **Creating**: `my_list = [1, 2, 3]`
- **Append**: `my_list.append(4)` adds an item to the end
- **Extend**: `my_list.extend([5, 6])` adds all elements of a list to another list
- **Insert**: `my_list.insert(1, 'a')` inserts an item at a given position
- **Remove**: `my_list.remove('a')` removes the first occurrence of an item
- **Pop**: `my_list.pop()` removes and returns the last item
- **Index**: `my_list.index('a')` returns the index of the first matched item
- **Count**: `my_list.count('a')` counts how many times an item appears
- **Sort**: `my_list.sort()` sorts the list in ascending order
- **Reverse**: `my_list.reverse()` reverses the elements of the list

#### Arrays
- **Import**: `from array import array`
- **Creating**: `arr = array('i', [1, 2, 3])` where 'i' is the type code for integers
- **Type Codes**: 'i' for integers, 'f' for floating points, etc.
- Operations like append, remove, and indexing work similarly to lists but are type-restricted.

#### Tuples
- **Immutable**: Once created, elements cannot be added, removed, or changed
- **Usage**: `my_tuple = (1, 2, 3)`

#### Sets
- **Creating**: `my_set = {1, 2, 3}`
- **Add**: `my_set.add(4)`
- **Remove**: `my_set.remove(2)`
- **Operations**: Union (`|`), Intersection (`&`), Difference (`-`), Symmetric Difference (`^`)

#### Dictionaries (More Details)
- **Creating**: `my_dict = {'key': 'value'}`
- **Accessing**: `my_dict['key']`
- **Adding/Updating**: `my_dict['new_key'] = 'new_value'`
- **Delete**: `del my_dict['key']`
- **Keys**: `my_dict.keys()` returns a list of keys
- **Values**: `my_dict.values()` returns a list of values
- **Items**: `my_dict.items()` returns a list of (key, value) tuples
- **Get**: `my_dict.get('key', default)` returns the value or a default if key is not found

### Comprehensions
- **List Comprehension**: `[x**2 for x in range(10)]`
- **Dict Comprehension**: `{k: v for k, v in zip(['a', 'b'], [1, 2])}`
- **Set Comprehension**: `{x for x in 'hello world' if x not in 'aeiou'}`

### Functions (More Details)
- **Default Parameters**: `def my_function(a=1, b=2):`
- **Keyword Arguments**: `my_function(b=3, a=2)`
- **Arbitrary Arguments**: `def my_function(*args):`
- **Arbitrary Keyword Arguments**: `def my_function(**kwargs):`

### Modules and Packages
- **Import a module**: `import math`
- **Import with alias**: `import numpy as np`
- **Import specific functions**: `from math import sqrt`
- **Custom Modules**: Create a Python file and import it using its filename

### Error Handling
- **Try/Except**: Catch exceptions to prevent crashes
- **Raise**: `raise ValueError('A message')` to throw an exception manually
- **Custom Exceptions**: Define your own exception classes inheriting from `Exception`

### File I/O (More Details)
- **Read Lines**: `lines = f.readlines()` to read all lines into a list
- **Write Lines**: `f.writelines(['Hello', 'World'])` to write a list of lines to a file
- **Modes**: 'r' (read), 'w' (write), 'a' (append), 'r+' (read/write)

### Decorators
- Used to modify the behavior of function or class
- **Syntax**: 
  ```python
  def my_decorator(func):
      def wrapper():
          # Do something before
          result = func()
          # Do something after
          return result
      return wrapper
  
  @my_decorator
  def my_function():
      pass
  ```

### Generators
- Functions that return an iterator that yields items instead of a single item
- **Syntax**: Use `yield` instead of `return`

```python


def my_generator():
    yield 'Hello'
    yield 'World'
```

