# Python_Programming
Introduction to python programming

## Introduction to Python Programming

Let's start with the basics of Python. Here's what we'll cover:

What is Python?

1. Variables and Data Types
2. Operators
3. Control Structures
4. Functions
5. Control Flow statements
6. Data Structures
7. File Input/Output in Python
8. Modules and Packages in Python

Once we cover these basics, we can move on to more advanced topics.

#### What is Python?

Python is a high-level programming language that is popular for its simplicity, readability, and versatility. It was created by Guido van Rossum in the late 1980s and has since become one of the most popular programming languages in the world. Python can be used for a wide range of applications, including web development, data analysis, machine learning, and more.

#### 1. Variables and Data Types

In Python, a variable is a container that holds a value. Values can be of different types, including:

- Integers: Whole numbers, such as 1, 2, 3, etc.
- Floats: Decimal numbers, such as 1.2, 3.4, etc.
- Strings: Text, such as "hello", "world", etc.
- Booleans: True or False.

To create a variable, you can use the following syntax:

`
variable_name = value
`
`
# Examples

x = 3 #integers

y = 2.5 # floats

name = "John" # strings

is_student = True # booleans
`

#### 2. Operators

Operators are used to perform operations on variables and values. There are several types of operators in Python, including:

**Arithmetic operators:** Used to perform arithmetic operations, such as addition (+), subtraction (-), multiplication (*), division (/), and modulus (%).

**Comparison operators:** Used to compare variables and values, such as equal to (==), not equal to (!=), greater than (>), less than (<), greater than or equal to (>=), and less than or equal to (<=).

**Logical operators:** Used to combine boolean expressions, such as and, or, and not.

**Assignment operators:** Used to assign values to variables, such as =, +=, -=, *=, /=, and %=.

`
# For example
# Arithmetic operators
x = 3 + 4   # x is now 7
y = 3 * 4   # y is now 12
`
`
# Comparison operators
a = 3
b = 4
print(a == b)   # False
print(a < b)    # True
`
`
# Logical operators
x = 5
y = 10
print(x < y and x > 0)   # True
print(x > y or x < 0)    # False
`
`
# Assignment operators
x = 5
x += 3    # x is now 8
x -= 2    # x is now 6
`

#### 3. Control Structures

Control structures are used to control the flow of a program. There are several types of control structures in Python, including:

**If statements:** Used to execute code if a condition is true.

**While loops:** Used to execute code repeatedly while a condition is true.

**For loops:** Used to iterate over a sequence of values.

`
# Examples
# If statement
x = 5
if x > 0:
    print("x is positive")
elif x == 0:
    print("x is zero")
else:
    print("x is negative")

# While loop
i = 0
while i < 5:
    print(i)
    i += 1

# For loop
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)
`
#### 4. Functions

Functions are used to group code that performs a specific task. They allow you to break up your code into reusable blocks, making it easier to read and maintain. In Python, you can define a function using the `def` keyword, followed by the function name and any parameters that it takes. 

Here's an example:
`
def greet(name):
    print("Hello, " + name + "!")

greet("Rodney")
`

The above function takes one parameter, `name`, and prints out a greeting using that name. When we call the function with `greet("Rodney")`, it will print out `"Hello, Rodney!"`.

Functions can also return values using the `return` keyword. 

Here's an example:
`
def square(x):
    return x * x

result = square(10)
print(result)
`
This function takes one parameter, `x`, and returns the square of that number. We call the function with `square(10)`, which returns `100`, and then we assign that result to the variable result and print it out.

Functions can also have default parameter values, which are used if the caller doesn't provide a value for that parameter. 

Here's an example:
`
def greet(name="world"):
    print("Hello, " + name + "!")

greet()        # prints "Hello, world!"
greet("Rodney")  # prints "Hello, Rodney!"
`

This function takes one optional parameter, `name`, which defaults to `"world"`. If we call the function with no arguments, it will use the default value and print out `"Hello, world!"`. If we call it with an argument, it will use that argument instead and print out `"Hello, Rodney!"`.

Finally, functions can also take variable-length arguments using the `*args` syntax. This allows you to pass in any number of arguments, which will be collected into a tuple. 

Here's an example:
`
def add(*args):
    result = 0
    for num in args:
        result += num
    return result
`
`
print(add(1, 2, 3))   # prints 6
print(add(1, 2, 3, 4))   # prints 10
print(add(0)) # prints 0
print(add()) # prints 0
`

This function takes any number of arguments, which are collected into the `args` tuple. It then adds up all of the numbers and returns the result. When we call the function with `add(1, 2, 3)`, it will return `6`, and when we call it with `add(1, 2, 3, 4)`, it will return `10`.

### 5. Control Flow statements

These include the following:

- if/else statements
- for loops
- while loops

Control flow statements allow you to control the flow of your program based on certain conditions or criteria. There are three types of control flow statements in Python: if/else statements, for loops, and while loops.

#### 1. if/else statements:

if/else statements allow you to execute certain code blocks if a certain condition is met, and a different code block if the condition is not met. The basic syntax for an if/else statement is as follows:

`
if condition:
    # code block to execute if the condition is true
else:
    # code block to execute if the condition is false
`
Below is an example:

`
x = 5
if x > 10:
    print("x is greater than 10")
else:
    print("x is less than or equal to 10")
`

This code block will output `"x is less than or equal to 10"` because the condition `x > 10` is false.

You can also use elif statements to check for additional conditions. 

The syntax for elif is similar to if:

`
if condition1:
    # code block to execute if condition1 is true
elif condition2:
    # code block to execute if condition2 is true
else:
    # code block to execute if neither condition1 nor condition2 are true
`
Below is an example:

`
x = 5
if x > 10:
    print("x is greater than 10")
elif x == 10:
    print("x is equal to 10")
else:
    print("x is less than 10")
`

This code block will output `"x is less than 10"` because the condition `x > 10` is false, and the condition `x == 10` is also false.

#### 2. for loops:

for loops allow you to iterate over a sequence of values, such as a list or a string, and execute a code block for each value. 

The basic syntax for a for loop is as follows:

`
for variable in sequence:
    # code block to execute for each value in the sequence
`
Below is an example:

`
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)
`
`
names = ["leo", "dante", "chinda", "salma", "zena", "neema"]
for n in names:
    print(n)
`

#### 3. while loops

while loops allow you to execute a code block repeatedly as long as a certain condition is true. The basic syntax for a while loop is as follows:

`
while condition:
    # code block to execute as long as the condition is true
`

Below is an example:
`
x = 0
while x < 5:
    print(x)
    x += 1
`
The code block in the while loop prints the current value of `x`, and then increments x by 1 using the `x += 1` shorthand for `x = x + 1`. This means that the first time the code block is executed, `x is equal to 0` and is printed to the console. 

Then, x is incremented to 1. The condition is still true `(1 < 5)`, so the code block is executed again, and x is printed to the console again. This process continues until `x is equal to 5`, at which point the condition is no longer true `(5 < 5 is false)`, and the while loop terminates.

So the output of the code block in the while loop is the sequence of values of x as it is incremented from 0 to 4.

### 6. Data Structures

Data structures are used to store and organize data in a way that makes it easy to access and manipulate. There are four main built-in data structures in Python: 

- lists
- tuples
- dictionaries
- sets.

#### 1. Lists:

A list is a collection of values that are ordered and mutable, meaning that you can add, remove, and modify elements in the list. The syntax for creating a list is to enclose a sequence of values in square brackets, separated by commas. 

For example:

`
fruits = ["apple", "banana", "cherry"]
`

You can access elements in a list by their index, which starts at 0. 

For example:
`
fruits = ["apple", "banana", "cherry"]
print(fruits[0])   # outputs "apple"
print(fruits[1])   # outputs "banana"
print(fruits[2])   # outputs "cherry"
`
You can also modify elements in a list by their index, like this:

`
fruits = ["apple", "banana", "cherry"]
fruits[1] = "orange"
print(fruits)   # outputs ["apple", "orange", "cherry"]
`
#### 2. Tupples

Tuples are similar to lists, but they are immutable, meaning they cannot be modified once they are created. Tuples are defined using parentheses instead of square brackets. 

Here's an example:

`
my_tuple = (1, 2, 3, "four", 5.6)
`
You can access elements of a tuple using the same syntax as for lists:

`
my_tuple = (1, 2, 3, "four", 5.6)
print(my_tuple[0]) # prints 1
print(my_tuple[3]) # prints "four"
`
However, you cannot modify the elements of a tuple:

`
my_tuple = (1, 2, 3, "four", 5.6)
my_tuple[1] = "two" # raises a TypeError: 'tuple' object does not support item assignment
`
#### 3. Dictionaries:

Dictionaries are used to store key-value pairs. Each key in a dictionary maps to a corresponding value. Dictionaries are defined using curly braces, with each key-value pair separated by a colon. 

Here's an example:

`
my_dict = {"name": "Rodney", "age": 24, "city": "Kilifi Kenya"}
`
You can access values in a dictionary using their keys:

`
my_dict = {"name": "Rodney", "age": 24, "city": "Kilifi Kenya"}
print(my_dict["name"]) # prints "Rodney"
print(my_dict["city"]) # prints "Kilifi Kenya"
print(my_dict["age"]) # prints 24
`

You can also modify values in a dictionary by assigning new values to their keys:

`
my_dict = {"name": "Rodney", "age": 24, "city": "New York"}
my_dict["age"] = 35
print(my_dict) # prints {"name": "John", "age": 35, "city": "New York"}
`

#### 4. Sets

Sets are used to store a collection of unique elements. Sets are defined using curly braces, with each element separated by a comma. 

Here's an example:

`
my_set = {1, 2, 3, 3, 4, 5, 5} # creates a set with unique elements
print(my_set) # prints {1, 2, 3, 4, 5}
`

You can perform various set operations, such as union, intersection, and difference, using set methods or operators.

1. Union: The union of two sets is a new set that contains all the elements from both sets, with duplicates removed. You can perform a union of two sets using the `union()` method or the `pipe (|) operator`.

2. Intersection: The intersection of two sets is a new set that contains only the elements that are common to both sets. You can perform an intersection of two sets using the `intersection()` method or the `ampersand (&) operator`.

3. Difference: The difference of two sets is a new set that contains only the elements that are in the first set but not in the second set. You can perform a difference of two sets using the `difference()` method or the `minus (-) operator`.

4. Symmetric difference: The symmetric difference of two sets is a new set that contains only the elements that are in one of the sets but not in both. You can perform a symmetric difference of two sets using the `symmetric_difference()` method or the `caret (^) operator`.

`
set1 = {1, 2, 3, 4}
set2 = {3, 4, 5, 6}

# union
print(set1.union(set2)) # prints {1, 2, 3, 4, 5, 6}
print(set1 | set2) # prints {1, 2, 3, 4, 5, 6}


# intersection
print(set1.intersection(set2)) # prints {3, 4}
print(set1 & set2) # prints {3, 4}


# difference
print(set1.difference(set2)) # prints {1, 2}
print(set1 - set2) # prints {1, 2}
`
You can also use set methods to add elements to a set or remove elements from a set:

`
my_set = {1, 2, 3}
my_set.add(4)
print(my_set) # prints {1, 2, 3, 4}

my_set.remove(3)
print(my_set) # prints {1, 2, 4}


# symmetric difference

set1 = {1, 2, 3}
set2 = {3, 4, 5}
symmetric_difference_set = set1.symmetric_difference(set2)
print(symmetric_difference_set) # Output: {1, 2, 4, 5}

# Alternatively, you can use the caret operator:
symmetric_difference_set = set1 ^ set2
print(symmetric_difference_set) # Output: {1, 2, 4, 5}
`

One important thing to note about sets is that they are unordered, meaning the elements are not stored in any particular order.

### 7. File Input/Output in Python

File I/O is an essential part of any programming language as it allows you to read from and write to files on your computer. In Python, there are several ways to work with files. Here are some of the most common methods:

**1. Opening a file:** 

To open a file, you can use the `open()` function, which takes **two arguments - the name of the file and the mode in which you want to open the file**. The mode can be `"r"` for *reading*, `"w"` for *writing*, or `"a"` for *appending* to an existing file.

Example:

`
*Open a file for reading*

file = open("example.txt", "r")

*Open a file for writing*

file = open("example.txt", "w")

*Open a file for appending*

file = open("example.txt", "a")
`
**2. Reading from a file:** 

To read from a file, you can use the `read()` method, which *reads the entire contents* of the file as a single string. You can also use the `readline()` method to read *a single line* from the file or the `readlines()` method to *read all the lines* in the file into a list.

Example:

`
*Read the entire file*

file = open("example.txt", "r")
contents = file.read()
print(contents)

*Read a single line*

file = open("example.txt", "r")
line = file.readline()
print(line)

*Read all lines into a list*

file = open("example.txt", "r")
lines = file.readlines()
print(lines)
`
**3 Writing to a file:** 

To write to a file, you can use the `write()` method, which *writes a string* to the file. You can also use the `writelines()` method to *write a list of strings* to the file.

Example:

`
*Write a string to the file*

file = open("example.txt", "w")
file.write("Hello, world!")
file.close()

*Write a list of strings to the file*

file = open("example.txt", "w")
lines = ["Hello", "world"]
file.writelines(lines)
file.close()
`
**4. Closing a file:** 

After you're done reading from or writing to a file, it's important to close the file using the `close()` method. This releases any system resources associated with the file and ensures that any changes you've made to the file are saved.

Example:
`
file = open("example.txt", "r")

Do some file operations

file.close()
`

### 8. Modules and Packages in Python

Python has a lot of built-in functions and data types, but sometimes you need more functionality than what is available out of the box. That's where modules and packages come in - they allow you to organize your code into reusable and shareable pieces.

A module is simply a file containing Python definitions and statements. You can define functions, classes, and variables in a module, and then use those definitions in other Python files by importing the module.

Here's an example of how to create and use a module:

1. Create a new file called my_module.py
2. Define some functions and variables in the file

`
*my_module.py*

def hello_world():
    print("Hello, world!")

def square(x):
    return x * x

message = "Welcome to my module!"
`

In another Python file, import the module and use its functions and variables

`
*import my_module*

my_module.hello_world() # prints "Hello, world!"

print(my_module.square(5)) # prints 25

print(my_module.message) # prints "Welcome to my module!"
`
Packages are simply directories that contain one or more Python modules. They allow you to organize related modules into a single namespace. When you import a package, Python looks for a file called `__init__.py` in the package directory, and executes the code in that file to initialize the package.

Here's an example of how to create and use a package:

1. Create a new directory called my_package
2. Inside the directory, create a file called `__init__.py`, which can be empty or contain initialization code
3. Create one or more module files in the directory

`
*my_package/module1.py*

def foo():
    print("Hello from module1!")

*my_package/module2.py*

def bar():
    print("Hello from module2!")
`
In another Python file, import the package and its modules and use their functions

`
*import my_package.module1*

*import my_package.module2*

my_package.module1.foo() # prints "Hello from module1!"

my_package.module2.bar() # prints "Hello from module2!"
`
That's a brief overview of how modules and packages work in Python. They are a powerful way to organize and reuse your code, and there are many Python libraries and frameworks available as modules and packages that you can use in your own projects.

### Excercises

1. Write a Python program that takes two numbers as input and prints their sum, difference, product, and quotient.

2. Write a Python program that takes a string as input and prints the reverse of the string.

3. Write a Python program that prints the first 20 Fibonacci numbers.

4. Write a Python program that takes a list of numbers as input and returns a new list containing only the even numbers from the original list.

5. Write a Python program that takes a list of words as input and returns a new list containing only the words that have an even number of letters.

6. Write a Python program that takes a list of integers as input and returns the largest and smallest numbers in the list.

7. Write a Python program that takes a string as input and counts the number of vowels in the string.

8. Write a Python program that takes a list of words as input and returns a new list containing only the words that start with a vowel.

9. Write a Python program that takes a list of numbers as input and returns a new list containing only the prime numbers from the original list.

10. Write a Python program that takes a sentence as input and returns a new sentence with the words in reverse order.

These exercises cover various concepts including input/output, string manipulation, loops, conditional statements, functions, and list comprehension. Good luck with practicing!

