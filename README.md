[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15338895&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.
   Python is a high level, interpreted, object-oriented, high-level programming language that can be used to create applications for different uses.
   key features
rapid development
versatility
easy integration
large ecosystem

web development, data science and machine learning, automation, scientific computing, education, research


2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.
   on a windows os
   Visit the link https://www.python.org/downloads/
   Select the Python's version to download.eg python 3.8.6
   Click on the Install Now
Double-click the executable file, which is downloaded;
Select Customize installation and proceed.
Click on the Add Path check box, it will set the Python path automatically.
verify- open command prompt
type 'python --version' you should see the installed version printed on the console
setting up a virtual environment
open command prompt
if 'virtualenv'is not installed, install it
navigate to the directory where you want to create the virtual environment
create the virtual environment
activate the virtual environment


3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.
  open your preferred python editor
  save a file with a .py extension eg 'hello_world.py'
  run the program.

   basic syntax elements
   comments- any beginning with '#'-used to document and explain the code
   print function'print()'- used to output data to the console or terminal. takes one or more arguments
   string laterals- strings are sequences of characters enclosed in either single or double quotes
   whitespace-spaces,tabs,new lines- are used to separate elements in the code
   function call'()'- the parenthesis are used to call a function.

4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.
integer(int)represents positive or negative whole numbers without any decimal point
   float- represents numbers with decimal point or exponent notation
   string- represents a sequence of characters enclosed within quotes, single or double quotes
   boolean(bool)-are values that can be either true or false, often used in conditiuonal statements
   list- are ordered collections of items that can be of any data type, i.e, strings, integers, floats
   noneType(none)a special data type that represents the absence of a value.

   # Create a string variable
name = "John Doe"
print("Hello, my name is", name)

# Create an integer variable
age = 30
print("I am", age, "years old")

# Create a float variable
height = 5.9
print("I am", height, "feet tall")

# Create a boolean variable
is_admin = True
print("I am an admin:", is_admin)

# Create a list variable
colors = ["red", "green", "blue"]
print("My favorite colors are:", colors)

# Create a dictionary variable
person = {"name": "John Doe", "age": 30, " occupation": "Developer"}
print("My name is", person["name"], "and I am a", person["occupation"])

# Use variables in a calculation
x = 5
y = 3
result = x + y
print("The result of", x, "+", y, "is", result)

# Use variables in a conditional statement
if is_admin:
    print("You have admin privileges")
else:
    print("You do not have admin privileges")

# Use variables in a loop
for color in colors:
    print("I like the color", color)
   


5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.
   conditional statements are used to execute different blocks of code based on certain conditions or decisions.
loops are used to execute a block of code repeatedly for a specified number of times.
'if-else' statement-
x = 10

if x > 5:
    print("x is greater than 5")
else:
    print("x is less than or equal to 5")

'for' loop
fruits = ["apple", "banana", "cherry"]

for fruit in fruits:
    print("I like to eat", fruit)



6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.
   a function is a block of code that can be executed multiple times from different parts of your program. functions are a powerful tool in that they can help you write more efficient, readable and maintainable code- code reusability, modularity,abstraction,,encapsulation,eaiser debugging, improved readability, improved perfomance
takes two arguments and returns their sum
def add_numbers(a, b):
    return a + b
how to call this function
result = add_numbers(3, 5)
print(result)  # Output: 8


7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.
   a list is a collection of items that can be of any data type.lists are ordered, indexed,mutable,homogenous or heterogenous. a list is used when you need to maintain a specific order, or when you need to perform operations sequentially
   a dictionary is an unordered collection of key value pairs, where each key is unique and maps to a specific value. dictionaries are unordered, key value pairs, mutable,homogenous keys. A dictionary is used when you need to store and retrieve data using unique keys or when you need to associate values with specific keys

# Create a list of numbers
numbers = [1, 2, 3, 4, 5]

# Create a dictionary with some key-value pairs
person = {
    "name": "John",
    "age": 30,
    "city": "New York"
}

# Demonstrate basic operations on the list
print("Original list:", numbers)

# Indexing: access a specific element
print("First element:", numbers[0])

# Slicing: access a range of elements
print("Middle elements:", numbers[1:3])

# Append: add a new element to the end
numbers.append(6)
print("List after appending:", numbers)

# Insert: add a new element at a specific position
numbers.insert(2, 2.5)
print("List after inserting:", numbers)

# Remove: remove the first occurrence of an element
numbers.remove(2)
print("List after removing:", numbers)

# Demonstrate basic operations on the dictionary
print("\nOriginal dictionary:", person)

# Access a value by its key
print("Name:", person["name"])

# Update a value
person["age"] = 31
print("Dictionary after updating:", person)

# Add a new key-value pair
person["country"] = "USA"
print("Dictionary after adding:", person)

# Remove a key-value pair
del person["city"]
print("Dictionary after removing:", person)


8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.
exception handling in python is a mechanism to handle runtime errors so that the normal flow of the application can be maintained. it allows the programmer to anticipate and handle errors that may occur during the execution of the program.
def divide_numbers(a, b):
    try:
        # Attempt to divide two numbers
        result = a / b
        print(f"The result of dividing {a} by {b} is {result}")
    except ZeroDivisionError:
        # Catch the ZeroDivisionError exception
        print("Error: Cannot divide by zero!")
    except TypeError:
        # Catch the TypeError exception
        print("Error: Invalid input type. Both inputs must be numbers.")
    finally:
        # Execute this block regardless of whether an exception was raised
        print("Division operation complete.")

# Test the function with valid inputs
divide_numbers(10, 2)

# Test the function with invalid inputs
divide_numbers(10, 0)  # Raises ZeroDivisionError
divide_numbers("10", 2)  # Raises TypeError
'try' blocks are used to wrap the code that might raise an exception
'except' blocks are used to catch specific exceptions that might be raised
'finally' blocks are used to execute some code regardless of whether an exception was raised or not


9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.
   a module is a single file that contains a collection of related functions,classes and variables. modules are used to organize and reuse code,making it easier to write and maintain large programs.
   a package is a collection of related modules and subpackages that are organized in a hierarchial structure.they are used to group related modules together making it easier to distribute and manage large collections of code.
   
   import and use a module- by using the 'import'statement

import math

# Calculate the sine of 3.14 radians
result = math.sin(3.14)
print(result)

# Calculate the value of pi
pi_value = math.pi
print(pi_value)


10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.
    you can read from and write to files using the built in 'open()'function,which returns a file object.
    read- use the 'open()'function to open the file in read mode
    use the 'read()'method to read the entire file contents as a string
    use the 'close()'method to close the file when youre done reading
    writinf to a file- use the 'open()'function to open the file in write mode(''w'')
use the 'write()'method to write a string to the file
use the 'close()'method to close the file when you are done writing

reads the contents and prints it to the console
# read_file.py

def read_file(filename):
    try:
        with open(filename, 'r') as file:
            content = file.read()
            print(content)
    except FileNotFoundError:
        print(f"Error: File '{filename}' not found.")

# Example usage:
read_file('example.txt')

writes a list of strings to the file
# write_file.py

def write_file(filename, strings):
    try:
        with open(filename, 'w') as file:
            for string in strings:
                file.write(string + '\n')
        print(f"Wrote to file '{filename}' successfully.")
    except IOError:
        print(f"Error: Unable to write to file '{filename}'.")

# Example usage:
strings = ["Hello", "World", "This is a test."]
write_file('example.txt', strings)




# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers. class notes, AI
- Submit your completed assignment by [due date].


