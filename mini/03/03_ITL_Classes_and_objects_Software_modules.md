Sure! Here are some independent tasks focused on Python classes and objects. Each task is designed to help you practice and deepen your understanding of OOP concepts in Python. 🐍💡

### Independent Tasks: Python Classes and Objects

#### Task 1: Create a `Rectangle` Class

1. **Define the class `Rectangle`** with attributes `length` and `width`.
2. Implement the following methods:
   - `area()`: Returns the area of the rectangle.
   - `perimeter()`: Returns the perimeter of the rectangle.
   - `is_square()`: Returns `True` if the rectangle is a square, otherwise `False`.

**Example Usage:**

```python
rect = Rectangle(10, 5)
print(rect.area())          # Output: 50
print(rect.perimeter())     # Output: 30
print(rect.is_square())     # Output: False
```

---

#### Task 2: Create a `Student` Class

1. Define the `Student` class with attributes `name`, `age`, and `grades` (a list of scores).
2. Implement the following methods:
   - `add_grade(grade)`: Adds a new grade to the grades list.
   - `average_grade()`: Returns the average of the grades.
   - `__str__()`: Returns a string representation of the student (name and average grade).

**Example Usage:**

```python
student = Student("Alice", 21)
student.add_grade(90)
student.add_grade(85)
print(student.average_grade())  # Output: 87.5
print(student)                   # Output: Alice's average grade is 87.5
```

---

#### Task 3: Create a `BankAccount` Class

1. Define a `BankAccount` class with attributes `account_number` and `balance`.
2. Implement the following methods:
   - `deposit(amount)`: Adds the specified amount to the balance.
   - `withdraw(amount)`: Deducts amount from balance if sufficient funds exist.
   - `get_balance()`: Returns the current balance.
   - `__str__()`: Returns a string representation of the account (account number and balance).

**Example Usage:**

```python
account = BankAccount("123456", 1000)
account.deposit(500)
print(account.get_balance())   # Output: 1500
account.withdraw(200)
print(account.get_balance())   # Output: 1300
print(account)                 # Output: Account 123456, Balance: 1300
```

---

#### Task 4: Create a `Book` Class

1. Create a `Book` class with attributes `title`, `author`, and `pages`.
2. Implement the following methods:
   - `read(pages_read)`: Updates the number of pages read, without exceeding the total pages.
   - `__str__()`: Returns a string representation of the book.

**Example Usage:**

```python
book = Book("1984", "George Orwell", 328)
book.read(100)
print(book)  # Output: 1984 by George Orwell, Pages read: 100/328
```

---

#### Task 5: Create an `Employee` Class

1. Define an `Employee` class with attributes `name`, `salary`, and `position`.
2. Implement the following methods:
   - `give_raise(amount)`: Increases the salary by the specified amount.
   - `change_position(new_position)`: Changes the employee's position.
   - `__str__()`: Returns a string representation of the employee's information.

**Example Usage:**

```python
employee = Employee("Bob", 50000, "Developer")
employee.give_raise(5000)
employee.change_position("Senior Developer")
print(employee)  # Output: Bob, Salary: 55000, Position: Senior Developer
```

---

### Bonus Task: Create a `MusicAlbum` Class

1. Define a `MusicAlbum` class with attributes `title`, `artist`, and `songs` (a list of song titles).
2. Implement the following methods:
   - `add_song(song_title)`: Adds a new song to the album.
   - `remove_song(song_title)`: Removes a song from the album if it exists.
   - `__str__()`: Returns a string representation of the album, including all songs.

**Example Usage:**

```python
album = MusicAlbum("Thriller", "Michael Jackson")
album.add_song("Billie Jean")
album.add_song("Beat It")
print(album)  # Output: Thriller by Michael Jackson, Songs: ['Billie Jean', 'Beat It']
```

---

These tasks allow you to practice defining classes, creating instance methods, and managing class attributes. Feel free to ask if you need assistance or feedback on your solutions! Happy coding! 😊📘

Here are some independent tasks focused on Python software modules. These tasks will help you understand how to create, use, and organize modules effectively. 📦✨

### Independent Tasks: Python Software Modules

#### Task 1: Create a Simple Math Module

1. **Create a module named `math_operations.py`** that defines the following functions:
   - `add(x, y)`: Returns the sum of `x` and `y`.
   - `subtract(x, y)`: Returns the difference of `x` and `y`.
   - `multiply(x, y)`: Returns the product of `x` and `y`.
   - `divide(x, y)`: Returns the quotient of `x` and `y`. Handle division by zero gracefully.

2. **Use the module** in a separate file (e.g., `main.py`) to demonstrate all four operations.

**Example Usage:**

```python
# In main.py
import math_operations as mo

print(mo.add(5, 3))         # Output: 8
print(mo.subtract(10, 4))   # Output: 6
print(mo.multiply(2, 3))     # Output: 6
print(mo.divide(8, 2))      # Output: 4.0
print(mo.divide(5, 0))      # Output: Cannot divide by zero!
```

---

#### Task 2: Create a String Utilities Module

1. **Create a module named `string_utils.py`** that includes the following functions:
   - `reverse_string(s)`: Returns the reversed version of the string `s`.
   - `count_vowels(s)`: Returns the number of vowels in the string `s`.
   - `to_uppercase(s)`: Returns the string `s` in uppercase.

2. **Use the module** in another file to demonstrate the string utility functions.

**Example Usage:**

```python
# In main.py
from string_utils import reverse_string, count_vowels, to_uppercase

print(reverse_string("hello"))                  # Output: olleh
print(count_vowels("hello world"))               # Output: 3
print(to_uppercase("hello"))                     # Output: HELLO
```

---

#### Task 3: Create a Statistics Module

1. **Create a module named `stats.py`** that provides the following functions:
   - `mean(numbers)`: Returns the mean (average) of a list of numbers.
   - `median(numbers)`: Returns the median of a list of numbers.
   - `mode(numbers)`: Returns the mode of a list of numbers.

2. **Use the module** in a separate Python file and test it with a list of numbers.

**Example Usage:**

```python
# In main.py
from stats import mean, median, mode

data = [1, 2, 2, 3, 4, 5, 5, 5]
print("Mean:", mean(data))       # Output: Mean: 3.125
print("Median:", median(data))   # Output: Median: 2.5
print("Mode:", mode(data))       # Output: Mode: 5
```

---

#### Task 4: Create a Conversion Module

1. **Create a module named `converter.py`** that includes functions for unit conversions:
   - `celsius_to_fahrenheit(c)`: Converts Celsius to Fahrenheit.
   - `fahrenheit_to_celsius(f)`: Converts Fahrenheit to Celsius.
   - `kilometers_to_miles(km)`: Converts kilometers to miles.

2. **Use the module** in a separate script to demonstrate the unit conversions.

**Example Usage:**

```python
# In main.py
from converter import celsius_to_fahrenheit, fahrenheit_to_celsius, kilometers_to_miles

print(celsius_to_fahrenheit(25))   # Output: 77.0
print(fahrenheit_to_celsius(77))    # Output: 25.0
print(kilometers_to_miles(5))       # Output: 3.106855
```

---

#### Task 5: Create a Package for Geometry

1. **Create a package named `geometry`,** which includes the following structure:
```
geometry/
    ├── __init__.py
    ├── shapes.py
    └── area_calculators.py
```

2. **In `shapes.py`**, define classes for `Circle` and `Rectangle` with methods to get their area.

3. **In `area_calculators.py`**, create functions to calculate the area of different shapes using the classes defined in `shapes.py`.

4. **Use the package** in a separate file (`main.py`) to demonstrate the area calculations.

**Example Usage:**

```python
# In main.py
from geometry.shapes import Circle, Rectangle
from geometry.area_calculators import calculate_circle_area, calculate_rectangle_area

circle = Circle(5)
rectangle = Rectangle(4, 6)

print("Circle Area:", calculate_circle_area(circle))        # Output: Circle Area: 78.53975
print("Rectangle Area:", calculate_rectangle_area(rectangle))  # Output: Rectangle Area: 24
```

---

These tasks will help you practice various aspects of defining and using Python modules effectively. If you have any questions or need feedback on your implementations, feel free to ask! Happy coding! 😊📘

