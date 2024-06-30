[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15348581&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.

   Python is a high-level programming language known for its readability and versatility. Its key features include simplicity, extensive libraries (like NumPy for scientific computing), and strong community support. Python excels in web development (Django), data analysis (Pandas), and automation (scripting tasks), making it ideal for everything from backend server applications to machine learning algorithms.

2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.

   
Installing Python:
(a). Windows: Download Python installer from python.org, run it, and select "Add Python to PATH" during installation.
   

Verifying Installation:
(a). Open Command Prompt  
(b). Type `python --version` or `python3 --version`. It should display the installed Python version.


This setup isolates Python dependencies for each project.

3. Python Syntax and Semantics:
   -Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.
   
```python
# This is a simple Python program that prints "Hello, World!" to the console.
print("Hello, World!")
```

Explanation:

(a). Comments (`#`): Comments in Python start with the `#` symbol. They are used for documentation and are ignored by the Python interpreter. In the example above, the comment `# This is a simple Python program that prints "Hello, World!" to the console.` provides a description of what the program does.

(b). Print Statement (`print()`): The `print()` function in Python is used to output text (or other objects) to the console. In this case, `print("Hello, World!")` prints the string `"Hello, World!"`. Strings in Python are enclosed in either single (`'`) or double (`"`) quotes.


4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.



(a). Integer (`int`): Represents whole numbers without decimal points (e.g., `5`, `-10`).
   
(b). Float (`float`): Represents numbers with decimal points (e.g., `3.14`, `2.5`).

(b). String (`str`): Represents sequences of characters, enclosed in quotes (`"` or `'`) (e.g., `"Hello"`, `'Python'`).

(b). Boolean (`bool`): Represents truth values, `True` or `False`, used in logical operations and conditions.

Short Script:
```python
# Define variables of different data types
my_integer = 10
my_float = 3.14
my_string = "Hello, Python!"
my_boolean = True

# Print the variables
print("Integer:", my_integer)
print("Float:", my_float)
print("String:", my_string)
print("Boolean:", my_boolean)
```



5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.

6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.

   Functions in Python: Functions in Python are reusable blocks of code that perform a specific task. They allow you to encapsulate functionality, making code more modular and easier to maintain.

Python Function Example:
```python
# Define a function that takes two arguments and returns their sum
def add_numbers(a, b):
    return a + b

# Example of calling the function
result = add_numbers(3, 5)
print("Sum:", result)  # Output: Sum: 8
```


7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.

  
(a). Lists: Lists are ordered collections of items that can contain duplicates. They are defined by square brackets (`[]`) and accessed by index. Example: `numbers = [1, 2, 3, 4]`.

(b). Dictionaries: Dictionaries are unordered collections of key-value pairs. Each key is unique and maps to a corresponding value, defined by curly braces (`{}`). Example: `person = {'name': 'Alice', 'age': 30}`.

Script Example:
```python
# Creating a list of numbers
numbers = [1, 2, 3, 4]

# Creating a dictionary of person's information
person = {'name': 'Alice', 'age': 30, 'city': 'New York'}

# Accessing elements
print("First number in list:", numbers[0])   # Output: 1
print("Person's age:", person['age'])       # Output: 30

# Modifying elements
numbers.append(5)                           # Adding an element to the list
person['city'] = 'San Francisco'            # Updating value in dictionary

# Displaying modified lists
print("Updated numbers list:", numbers)     # Output: [1, 2, 3, 4, 5]
print("Updated person dictionary:", person) # Output: {'name': 'Alice', 'age': 30, 'city': 'San Francisco'}
```



8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.

Exception handling in Python: Exception handling in Python allows for graceful management of errors that may occur during program execution. It involves using `try`, `except`, and optionally `finally` blocks to handle and respond to exceptions.

ilustration
```python
# Example of exception handling
try:
    result = 10 / 0  # This will raise a ZeroDivisionError
except ZeroDivisionError as e:
    print("Error:", e)  # Handle specific exception
finally:
    print("Execution completed.")  # Optional block for cleanup or final tasks
```



9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.

Modules and packages in Python: Modules are individual files containing Python code, while packages are directories of modules. They organize code into reusable units and facilitate modular programming.

Example with `math` module:
```python
# Example of importing and using the math module
import math

print("Square root of 16 is:", math.sqrt(16))  # Output: Square root of 16 is: 4.0
```



10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.

Reading from and writing to files in Python: To read from a file, use `open()` with mode `'r'` or `'rt'`. To write to a file, use `'w'` or `'wt'`. 

Example for reading from a file:
```python
# Reading from a file and printing its content
with open('example.txt', 'r') as file:
    content = file.read()
    print(content)
```

Example for writing to a file:
```python
# Writing a list of strings to a file
data = ['Apple', 'Banana', 'Cherry']

with open('fruits.txt', 'w') as file:
    for item in data:
        file.write(item + '\n')
```


# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].


