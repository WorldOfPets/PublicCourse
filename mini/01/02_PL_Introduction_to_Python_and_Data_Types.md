### Practical Lesson: Introduction to Python and Data Types 🐍🔍

In this practical lesson, we will explore Python's syntax and data types by engaging in hands-on exercises. Make sure you have Python installed on your computer, or you can use an online coding platform (like Jupyter Notebook, Google Colab, or Repl.it) to follow along. Let’s get started! 🚀

---

#### **Objective**
By the end of this lesson, you will:
- Understand Python syntax and how to run Python code.
- Be able to create and manipulate different data types: lists, dictionaries, tuples, and sets.

---

### Part 1: Setting Up Your Environment 🖥️

1. **Open your coding environment** (local Python IDE or online platform).
2. **Create a new Python file or notebook**.

---

### Part 2: Basic Python Syntax 📜

Before diving into data types, let’s look at some basic syntax. 

#### **Exercise 1: Print Statement**
```python
# Print a message to the console
print("Hello, Python!")
```

#### **Task**: Run this code and observe the output. 

---

### Part 3: Data Types in Python 🍏

#### **1. Lists 📜**

**Example Code:**
```python
# Create a list of mixed data types
my_list = [1, "Python", 3.14, True]
print("Original List:", my_list)
```

**Exercises:**
1. Access the second element of the list.
   ```python
   print("Second element:", my_list[1])
   ```
2. Add an element to the list.
   ```python
   my_list.append("New Item")
   print("Updated List:", my_list)
   ```
3. Remove the first element from the list.
   ```python
   my_list.remove(1)
   print("List after removing 1:", my_list)
   ```

---

#### **2. Dictionaries 📚**

**Example Code:**
```python
# Create a dictionary with key-value pairs
my_dict = {"name": "Alice", "age": 30, "city": "New York"}
print("Original Dictionary:", my_dict)
```

**Exercises:**
1. Access the value associated with the key "age".
   ```python
   print("Age:", my_dict["age"])
   ```
2. Add a new key-value pair for "email".
   ```python
   my_dict["email"] = "alice@example.com"
   print("Updated Dictionary:", my_dict)
   ```
3. Remove the key "city" from the dictionary.
   ```python
   del my_dict["city"]
   print("Dictionary after removing city:", my_dict)
   ```

---

#### **3. Tuples ⛰️**

**Example Code:**
```python
# Create a tuple
my_tuple = (10, 20, 30, "Hello")
print("Original Tuple:", my_tuple)
```

**Exercises:**
1. Access the third element of the tuple.
   ```python
   print("Third element:", my_tuple[2])
   ```
2. Print the length of the tuple.
   ```python
   print("Length of tuple:", len(my_tuple))
   ```

---

#### **4. Sets 🥳**

**Example Code:**
```python
# Create a set of numbers
my_set = {1, 2, 3, 4, 5}
print("Original Set:", my_set)
```

**Exercises:**
1. Add a new number to the set.
   ```python
   my_set.add(6)
   print("Set after adding 6:", my_set)
   ```
2. Remove a number from the set.
   ```python
   my_set.remove(3)
   print("Set after removing 3:", my_set)
   ```
3. Check if a value exists in the set.
   ```python
   print("Is 2 in the set?", 2 in my_set)
   ```

---

### Part 4: Summary and Discussion 📝

1. **Review Your Work**: Go through the exercises you completed and ensure you've noted the outputs.
2. **Key Takeaways**:
   - Lists are ordered and mutable.
   - Dictionaries are key-value pairs.
   - Tuples are ordered but immutable.
   - Sets are unordered collections of unique items.

---

### Part 5: Optional Challenge 💡

Create a small program that combines what you've learned:

1. Create a list of three favorite fruits.
2. Create a dictionary that includes your name, age, and favorite fruit from that list.
3. Print out the dictionary.
4. Use a tuple to store your favorite numbers and print it.
5. Create a set of at least five unique colors, add a new color, and check if a specific color is in the set.

**Example Structure:**
```python
# Your Code Here
```

---

### Conclusion 🎉

Congratulations on completing this practical lesson on Python and its data types! Feel free to ask questions or seek clarification on any topic. Keep practicing to enhance your understanding and skills! 😊
