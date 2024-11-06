Here are some independent tasks focused on Python file handling and exception handling. These tasks will help reinforce understanding of both concepts through practical application. 📝🐍

### Independent Tasks: Python File Handling and Exception Handling

#### Task 1: File Reading and Writing
1. **Create a New Text File**:
   - Write a Python program that creates a new text file named `tasks.txt`.
   - Write three lines of text into the file, each representing a different task.

2. **Read from the Text File**:
   - Extend your program to read the content of `tasks.txt` line by line and print each line to the console.

3. **Append to the File**:
   - Modify the program to append a fourth task to the file after reading the existing ones.
   - The fourth task should be user-provided input.

#### Task 2: File Management
1. **Copy File Content**:
   - Write a Python script that copies the content of `tasks.txt` to a new file named `tasks_copy.txt`.
   - Ensure that the new file is created in the same directory.

2. **File Existence Check**:
   - Before performing the copy operation, check if `tasks.txt` exists. If it doesn’t, print a message to the console indicating the file was not found.

#### Task 3: Exception Handling
1. **Handling File Not Found Error**:
   - Create a program that attempts to open and read a file named `data.txt`.
   - Implement exception handling to catch the `FileNotFoundError` and print a meaningful error message.

2. **Handling General Exceptions**:
   - Extend the program to handle other potential exceptions (such as `IOError`).
   - Use a generic `except Exception as e:` block to catch any unexpected exceptions and display the error message.

#### Task 4: Writing and Reading Data with Exception Handling
1. **Writing User Input to a File**:
   - Write a program that asks the user for their name and age and saves this information into a file named `user_data.txt`.
   - Use exception handling to manage potential issues (e.g., data not being written due to file permissions).

2. **Reading User Data from File**:
   - After writing to the file, read the content of `user_data.txt` and print the user details to the console.
   - Handle exceptions that may arise if the file doesn’t exist.

#### Task 5: CSV File Handling
1. **Create a CSV File**:
   - Write a Python script to create a CSV file named `employees.csv` containing the following columns: `Name`, `Age`, `Department`.
   - Populate the CSV file with at least 5 entries.

2. **Read the CSV File**:
   - Create another script to read the `employees.csv` file and print each row in a readable format (e.g., "Name: John Doe, Age: 30, Department: HR").
   - Include exception handling to manage scenarios where the CSV file cannot be found or read.

#### Task 6: Log File Creation
1. **Writing Log Entries**:
   - Create a logging function that appends log messages to a file named `log.txt`.
   - The function should accept a log message and include a timestamp.

2. **Reading Log Entries**:
   - Write a script to read and display the contents of `log.txt`, ensuring that exception handling is in place for file operations.

---

### Submission Guidelines
- Each task should be completed in separate Python scripts.
- Include comments in your code to explain important sections.
- Test your code to ensure it handles exceptions properly.
- Submit the scripts and a brief report (1-2 paragraphs) on your experience, including any challenges faced and how you resolved them.

These tasks are designed to build practical skills in file and exception handling in Python, while also encouraging students to implement best coding practices. If you have any specific preferences or need adjustments, let me know! 😊
