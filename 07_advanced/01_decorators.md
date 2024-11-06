Here’s a structured outline for lecture material on the topic of "Python Decorators and Their Uses." This will cover the definition, implementation, and practical applications of decorators in Python. 🎓🐍

---

### Lecture Title: Python Decorators and Their Uses

#### 1. Introduction to Decorators
   - **Definition**: A decorator is a function that modifies or enhances another function or method. It is a higher-order function that takes a function as an argument and returns another function.
   - **Purpose**: To add functionality to existing functions in a clean and concise manner, without modifying their structure.

#### 2. The Basics of Functions in Python
   - **First-Class Functions**: Functions in Python are first-class citizens, which means they can be passed around as arguments, returned from other functions, and assigned to variables.
   - **Example**:
     ```python
     def greet(name):
         return f"Hello, {name}!"

     print(greet("Alice"))  # Hello, Alice!
     ```

#### 3. The Simple Decorator
   - **Creating a Basic Decorator**:
     - Structure of a decorator function.
     - Using the `@decorator_name` syntax to apply a decorator.
   - **Example of a Simple Decorator**:
     ```python
     def my_decorator(func):
         def wrapper():
             print("Something is happening before the function is called.")
             func()
             print("Something is happening after the function is called.")
         return wrapper

     @my_decorator
     def say_hello():
         print("Hello!")

     say_hello()
     ```
   - **Expected Output**:
     ```
     Something is happening before the function is called.
     Hello!
     Something is happening after the function is called.
     ```

#### 4. Using Arguments with Decorators
   - **Passing Arguments**: Modify the decorator to accept arguments for the wrapped function.
   - **Example**:
     ```python
     def repeat(num_times):
         def decorator_repeat(func):
             def wrapper(*args, **kwargs):
                 for _ in range(num_times):
                     func(*args, **kwargs)
             return wrapper
         return decorator_repeat

     @repeat(num_times=3)
     def greet(name):
         print(f"Hello, {name}!")

     greet("Alice")
     ```
   - **Expected Output**:
     ```
     Hello, Alice!
     Hello, Alice!
     Hello, Alice!
     ```

#### 5. Common Use Cases of Decorators
   - **Logging**: Tracking function calls and parameters for debugging or auditing.
   - **Authorization**: Checking user permissions before allowing access to a function.
   - **Caching**: Storing results of expensive function calls to improve performance.
   - **Input Validation**: Checking input parameters before executing the main function logic.

#### 6. Practical Examples
   - **Example 1: Logging Decorator**:
     ```python
     def log_function_call(func):
         def wrapper(*args, **kwargs):
             print(f"Calling function {func.__name__} with arguments {args} and {kwargs}")
             return func(*args, **kwargs)
         return wrapper

     @log_function_call
     def add(a, b):
         return a + b

     add(5, 10)
     ```

   - **Example 2: Caching Results**:
     ```python
     cache = {}
     def cache_decorator(func):
         def wrapper(*args):
             if args in cache:
                 return cache[args]
             result = func(*args)
             cache[args] = result
             return result
         return wrapper

     @cache_decorator
     def compute_square(n):
         return n * n

     print(compute_square(4))
     print(compute_square(4))  # This will use the cached result
     ```

#### 7. Decorators with Parameters: A Deeper Dive
   In Python, `functools.wraps` is a decorator that is part of the `functools` module. It is primarily used when you create a decorator function, and it helps preserve the metadata of the original function that is being wrapped. 🏷️✨

#### Purpose of `functools.wraps`

When you define a decorator, it typically replaces the original function with the wrapper function. As a consequence, the attributes of the original function (such as its name, docstring, and other metadata) are lost unless you explicitly copy them. `functools.wraps` automatically copies this metadata from the original function to the wrapper function.

#### Key Attributes Preserved by `functools.wraps`

- **`__name__`**: The name of the function.
- **`__doc__`**: The docstring of the function.
- **`__module__`**: The module in which the function was defined.
- Additionally, it can preserve other attributes if set similarly.

#### Example of Using `functools.wraps`

Here’s an example to demonstrate how to use `functools.wraps` in a custom decorator:

```python
import functools

def my_decorator(func):
    @functools.wraps(func)  # This preserves the metadata of 'func'
    def wrapper(*args, **kwargs):
        print("Before the function call.")
        result = func(*args, **kwargs)
        print("After the function call.")
        return result
    return wrapper

@my_decorator
def say_hello(name):
    """This function greets a person."""
    print(f"Hello, {name}!")

# Using the decorated function
say_hello("Alice")

# Accessing metadata
print(say_hello.__name__)  # Output: say_hello
print(say_hello.__doc__)   # Output: This function greets a person.
```

#### Explanation of the Example

1. **Defining the Decorator**:
   - `my_decorator` is a decorator that takes a function `func` as an argument and defines a `wrapper` function around it.

2. **Using `@functools.wraps(func)`**:
   - By applying `@functools.wraps(func)` to the `wrapper` function, the original function's metadata (like its name and docstring) is copied to the `wrapper`.

3. **Using the Decorator**:
   - When we decorate `say_hello` with `@my_decorator`, the original function remains accessible under the same name, and the metadata is preserved.

4. **Calling the Function**:
   - When you call `say_hello("Alice")`, you see the print statements from the decorator as well as the function’s output.

5. **Accessing Metadata**:
   - The printed name and docstring confirm that the metadata has been preserved, showcasing the importance of using `functools.wraps` in a decorator.


#### 8. Conclusion
   - Recap the concept of decorators, their syntax, and their practical uses.
   - Emphasize how decorators promote code reusability and separation of concerns.
   - Encourage practice in implementing custom decorators.

#### 9. Q&A Session
   - Open the floor for questions to clarify any concepts and allow for discussion.

### Additional Tips:
- Incorporate visual aids like flowcharts to explain how decorators work.
- Use interactive coding examples where possible to engage the audience.
- Provide exercises to implement different types of decorators as homework or practice.

---

Feel free to adapt this outline based on your audience's needs or specific focus areas! If you need further details on any topic or clarification, just let me know! 😊
