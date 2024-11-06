Here are some independent tasks focused on the topic of Python functions and modules. These tasks will help learners practice and reinforce their understanding of how to define and use functions and modules effectively. 🐍💻

### Independent Tasks: Python Functions and Modules

#### Task 1: Define and Call Functions
1. **Create a Function**: Write a function called `calculate_area` that takes two parameters: `length` and `width`. The function should return the area of a rectangle.
   ```python
   def calculate_area(length, width):
       # Your code here
   ```

2. **Function Call**: Call the function with different sets of values and print the results.

#### Task 2: Use Default Parameters
1. **Create a Function with Default Values**: Write a function called `greet` that takes one parameter `name` with a default value of "Guest". The function should print a greeting message.
   ```python
   def greet(name="Guest"):
       # Your code here
   ```

2. **Test the Function**: Call the function with and without an argument to see how it behaves.

#### Task 3: Return Multiple Values
1. **Create a Function**: Write a function named `get_stats` that takes a list of numbers as an argument and returns the minimum, maximum, and average of the list.
   ```python
   def get_stats(numbers):
       # Your code here
   ```

2. **Test the Function**: Create a list of numbers and print the results returned by the function.

#### Task 4: Explore Variable Scope
1. **Understand Scope**: Write a function named `scope_test` that modifies a global variable and a local variable. Print the values inside and outside the function to observe the scope.
   ```python
   global_var = 10

   def scope_test():
       local_var = 5
       global global_var
       global_var += 5
       print("Inside function:", local_var, global_var)

   scope_test()
   print("Outside function:", global_var)
   ```

#### Task 5: Create a Module
1. **Create a Module**: Write a Python file called `math_operations.py` that contains the following functions:
   - `add(a, b)`
   - `subtract(a, b)`
   - `multiply(a, b)`
   - `divide(a, b)`

2. **Function Implementation**: Implement the functions to perform their respective operations.

3. **Import the Module**: In a separate Python file, import the `math_operations` module and demonstrate the use of each function with example values.

#### Task 6: Use Built-in Modules
1. **Random Number Generation**: Write a script that:
   - Uses the `random` module to generate and print five random numbers between 1 and 100.
   - Uses the `math` module to calculate and print the square root of one of the random numbers.

   ```python
   import random
   import math

   # Your code here
   ```

#### Task 7: Exception Handling in Functions
1. **Create a Robust Function**: Write a function called `safe_divide` that takes two numbers and returns their division result. Implement exception handling to manage division by zero.
   ```python
   def safe_divide(a, b):
       # Your code here
   ```

2. **Test the Function**: Call the function with both valid and invalid inputs, and print the results.

#### Task 8: Documentation and Comments
1. **Document Your Functions**: Take any of your previous functions and add docstrings to explain what the function does, its parameters, and its return value.

   ```python
   def example_function(param1, param2):
       """
       Function description: 
       Args:
           param1: Description of param1
           param2: Description of param2
       Returns:
           Description of return value
       """
       # Your code here
   ```

#### Task 9: Your Own Utility Module
1. **Create a Custom Utility Module**: Design a Python module that includes functions for common tasks, such as:
   - Converting temperature from Celsius to Fahrenheit and vice versa.
   - Calculating the factorial of a number.
   - Checking if a number is prime.
   
2. **Demonstrate Usage**: In a separate script, import your utility module and use each function with example inputs.

---

Feel free to modify the tasks according to your audience's skill level, and encourage them to explore and experiment beyond the requirements! Let me know if you need further assistance or additional tasks! 😊
