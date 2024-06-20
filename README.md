[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15305685&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.

  Python is a high-level, interpreted programming language known for its readability and versatility. Some key features include:
  - **Easy to Read and Write:** Python syntax is clear and concise, making it easy to learn and use.
  - **Interpreted Language:** Python code is executed line by line, which simplifies debugging.
  - **Dynamic Typing:** Variable types are determined at runtime, allowing for flexible and rapid development.
  - **Extensive Standard Library:** Python comes with a wide range of modules and packages that facilitate various tasks.
  - **Community Support:** A large and active community provides extensive resources and libraries.

  **Use Cases:**
  - **Web Development:** Using frameworks like Django and Flask.
  - **Data Analysis and Visualization:** Libraries like Pandas, NumPy, and Matplotlib.
  - **Machine Learning:** Libraries such as TensorFlow and scikit-learn.
  - **Automation and Scripting:** Writing scripts for automating repetitive tasks.


2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.

  **Installing Python on Windows:**
  1. Download the Python installer from the official website (https://www.python.org/).
  2. Run the installer and check the box to add Python to PATH.
  3. Follow the installation prompts.

  **Verifying Installation:**
  ```sh
  python --version
  ```

  **Setting up a Virtual Environment:**
  ```sh
  python -m venv myenv
  source myenv/Scripts/activate  # On Windows
  source myenv/bin/activate      # On macOS/Linux
  ```


3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.

  ```python
  print("Hello, World!")
  ```

  **Explanation:**
  - `print`: A built-in function to output text to the console.
  - `"Hello, World!"`: A string literal enclosed in double quotes.


4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.


  **Basic Data Types:**
  - `int`: Integer numbers
  - `float`: Floating-point numbers
  - `str`: Strings (text)
  - `bool`: Boolean values (True or False)
  - `list`: Ordered, mutable collection
  - `tuple`: Ordered, immutable collection
  - `dict`: Unordered, mutable collection of key-value pairs

  ```python
  x = 10          # int
  y = 3.14        # float
  name = "Austin"  # str
  is_active = True  # bool
  numbers = [1, 2, 3]  # list
  point = (1, 2)  # tuple
  user = {"name": "Austin", "age": 21}  # dict

  print(x, y, name, is_active)
  print(numbers, point, user)
  ```
5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.

  **Conditional Statements:**
  ```python
  age = 20
  if age >= 18:
      print("Adult")
  else:
      print("Minor")
  ```

  **Loops:**
  ```python
  for i in range(5):
      print(i)

  total = 0
  while total < 5:
      print(total)
      total += 1
  ```


6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.

  Functions are reusable blocks of code that perform a specific task. They promote modularity and code reuse.

  ```python
  def add(a, b):
      return a + b

  result = add(3, 5)
  print(result)  # Output: 8
  ```


7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.

  **Differences:**
  - Lists are ordered collections accessed by index.
  - Dictionaries are unordered collections accessed by key.

  ```python
  numbers = [1, 2, 3, 4, 5]
  user = {"name": "Austin", "age": 21}

  # List operations
  numbers.append(6)
  print(numbers)

  # Dictionary operations
  user["email"] = "kuriaaustin125@gmail.com"
  print(user)
  ```
8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.

Exception handling manages errors and exceptions gracefully without crashing the program.

  ```python
  try:
      result = 10 / 0
  except ZeroDivisionError as e:
      print("Error:", e)
  finally:
      print("This block always executes.")
  ```

9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.

  - **Modules:** Files containing Python code (functions, classes).
  - **Packages:** Collections of modules organized in directories.

  **Importing and Using a Module:**
  ```python
  import math

  print(math.sqrt(16))  # Output: 4.0
  ```


10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.

  **Reading from a File:**
  ```python
  with open("example.txt", "r") as file:
      content = file.read()
      print(content)
  ```

  **Writing to a File:**
  ```python
  lines = ["Hello", "World"]
  with open("output.txt", "w") as file:
      for line in lines:
          file.write(line + "\n")
  ```


# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].