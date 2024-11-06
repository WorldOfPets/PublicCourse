Here are some independent tasks focused on Object-Oriented Programming (OOP) in Python. These tasks are designed to help learners practice key OOP concepts such as classes, objects, inheritance, encapsulation, and polymorphism. 🐍✨

### Independent Tasks on Python OOP

#### Task 1: Class Creation and Object Instantiation
- **Objective**: Create a class named `Car`.
  - Define attributes: `make`, `model`, `year`, and `color`.
  - Create a method called `display_info()` that prints the car's details.
  - Instantiate at least two objects of the `Car` class and call the `display_info()` method for each.

#### Task 2: Implementing Inheritance
- **Objective**: Build a class structure for a simple vehicle system.
  - Create a base class `Vehicle` with attributes for `make`, `model`, and `year`.
  - Create a derived class `Bike` that inherits from `Vehicle` and adds an attribute `type` (e.g., mountain, road).
  - Implement a method `display_info()` in both classes to show their details, then instantiate both classes and demonstrate inheritance by calling the methods.

#### Task 3: Encapsulation
- **Objective**: Modify the `Car` class to demonstrate encapsulation.
  - Make attributes `make`, `model`, `year`, and `color` private.
  - Create getter and setter methods for each attribute.
  - Implement input validation in the setter methods (e.g., ensure `year` is a four-digit number).
  - Instantiate the class and test the getters and setters.

#### Task 4: Polymorphism
- **Objective**: Illustrate polymorphism by defining multiple classes that implement a common method.
  - Create a class `Dog` with a method `speak()` that returns "Woof!".
  - Create another class `Cat` with a method `speak()` that returns "Meow!".
  - Create a function `animal_sound(animal)` that takes an animal object and prints the result of calling `animal.speak()`. Test this function with both `Dog` and `Cat` objects.

#### Task 5: Class Composition and Relationships
- **Objective**: Create a class that demonstrates composition.
  - Define a class `Engine` with attributes `horsepower` and `type`.
  - Define the `Car` class to have an attribute of type `Engine`.
  - Implement a method in the `Car` class that calls a method from the `Engine` class to display engine details.
  - Instantiate a `Car` with an `Engine` and demonstrate the relationship.

#### Task 6: Abstract Classes and Interfaces
- **Objective**: Use abstract classes to enforce a contract for subclasses.
  - Import the `ABC` module from Python’s `abc` library to define an abstract class `Shape`.
  - Define an abstract method `area()` that must be implemented by any subclass.
  - Create subclasses `Circle` and `Rectangle` that implement the `area()` method.
  - Instantiate objects of both subclasses and print their areas.

#### Task 7: Real-World OOP Project
- **Objective**: Consolidate your knowledge of OOP principles by creating a small project.
  - Choose a real-world scenario (e.g., a library system, a zoo management system, or a bank account management system).
  - Identify the necessary classes and their relationships (use inheritance, encapsulation, and polymorphism where relevant).
  - Implement the classes, methods, and attributes.
  - Create instances and demonstrate interactions among the objects.

### Writing Guidelines
- Encourage learners to write clean, well-documented code.
- Suggest using comments to explain the purpose of methods and classes.
- Recommend testing each task's functionality with relevant examples.

### Conclusion
These independent tasks are designed to progressively build skills in Python OOP concepts. Completing them will help solidify knowledge and prepare learners for more advanced programming challenges. If you need further refinement or more tasks, feel free to ask! 😊
