# Python-Viva
# Basic Questions:

### What is Python, and why is it popular?
Python is a high-level, interpreted programming language known for its simplicity and readability. It is popular because of its easy-to-understand syntax, extensive standard library, and versatility in various fields such as web development, data science, artificial intelligence, and more.

### How do you take user input in Python?
You can take user input in Python using the `input()` function. For example:
```python
user_input = input("Enter something: ")
```

### What are the different data types in Python?
The different data types in Python include:
- `int` (integer)
- `float` (floating-point number)
- `str` (string)
- `bool` (boolean)
- `list`
- `tuple`
- `set`
- `dict` (dictionary)

### What is the difference between `int`, `float`, and `str` in Python?
- `int`: Represents whole numbers without a fractional part.
- `float`: Represents numbers with a fractional part.
- `str`: Represents sequences of characters (strings).

### How do you perform type conversion in Python?
You can perform type conversion using built-in functions like `int()`, `float()`, and `str()`. For example:
```python
num_str = "123"
num_int = int(num_str)
num_float = float(num_str)
```

### What are arithmetic operators in Python? Can you name a few?
Arithmetic operators in Python are used to perform mathematical operations. Some examples include:
- `+` (addition)
- `-` (subtraction)
- `*` (multiplication)
- `/` (division)
- `%` (modulus)
- `**` (exponentiation)

### How do you print output in Python?
You can print output in Python using the `print()` function. For example:
```python
print("Hello, World!")
```

### What is the difference between `print()` and `input()`?
- `print()`: Outputs data to the console.
- `input()`: Takes input from the user.

### What are keywords in Python? Can you name some?
Keywords are reserved words in Python that have special meanings. Some examples include `if`, `else`, `while`, `for`, `break`, `continue`, `def`, `return`, `class`, `try`, `except`.

### What is the significance of indentation in Python?
Indentation in Python is used to define the scope of code blocks. It is crucial for the proper execution of control flow statements like loops and conditionals.

# Syntax & Logical Questions:

### What is the correct syntax for an `if-else` statement?
```python
if condition:
    # code block
else:
    # code block
```

### How does an `elif` statement work?
The `elif` statement allows you to check multiple conditions sequentially. If the first condition is false, it checks the next `elif` condition, and so on. For example:
```python
if condition1:
    # code block
elif condition2:
    # code block
else:
    # code block
```

### What is the purpose of using `round()` in mathematical calculations?
The `round()` function is used to round a floating-point number to a specified number of decimal places. For example:
```python
rounded_number = round(3.14159, 2)  # Output: 3.14
```

### Why do we use `float(input())` instead of `int(input())` in some cases?
We use `float(input())` when we expect the user to enter a floating-point number. `int(input())` is used when we expect an integer.

### What is the purpose of using `str()` in input operations?
The `str()` function is used to convert a value to a string, which can be useful for concatenating with other strings or for display purposes.

### How can you format output in Python?
You can format output using f-strings, the `format()` method, or the `%` operator. For example:
```python
name = "Alice"
age = 30
print(f"Name: {name}, Age: {age}")
```

### What happens if you divide by zero in Python?
Dividing by zero raises a `ZeroDivisionError` exception.

### How can you check if a number is even or odd?
You can check if a number is even or odd using the modulus operator `%`. For example:
```python
number = 10
if number % 2 == 0:
    print("Even")
else:
    print("Odd")
```

### What is the difference between `=` and `==`?
- `=`: Assignment operator, used to assign a value to a variable.
- `==`: Equality operator, used to compare two values for equality.

### Why do we use `//` instead of `/` for division in some cases?
The `//` operator performs integer division, which returns the quotient without the fractional part. The `/` operator performs floating-point division, which returns a float.

# Conditional Statements & Loops:

### What are conditional statements in Python?
Conditional statements are used to execute different code blocks based on certain conditions. Examples include `if`, `elif`, and `else`.

### What is the purpose of `if`, `elif`, and `else`?
- `if`: Executes a code block if the condition is true.
- `elif`: Checks another condition if the previous `if` condition is false.
- `else`: Executes a code block if all previous conditions are false.

### How does a `while` loop work?
A `while` loop repeatedly executes a code block as long as the given condition is true. For example:
```python
count = 0
while count < 5:
    print(count)
    count += 1
```

### What is the difference between a `for` loop and a `while` loop?
- `for` loop: Iterates over a sequence (e.g., list, range) and executes a code block for each item.
- `while` loop: Repeatedly executes a code block as long as a condition is true.

### How can you iterate over a range of numbers in Python?
You can use the `range()` function with a `for` loop. For example:
```python
for i in range(5):
    print(i)
```

### How do you find the sum of the first `n` natural numbers using a loop?
```python
n = 10
sum = 0
for i in range(1, n + 1):
    sum += i
print(sum)
```

### What is the difference between `break` and `continue`?
- `break`: Exits the loop immediately.
- `continue`: Skips the current iteration and continues with the next iteration.

### How do you swap two numbers without using a third variable?
```python
a = 5
b = 10
a, b = b, a
```

### What is recursion? Can you give an example?
Recursion is a programming technique where a function calls itself. Example:
```python
def factorial(n):
    if n == 0:
        return 1
    else:
        return n * factorial(n - 1)
```

### How do you determine if a number is prime using a loop?
```python
def is_prime(n):
    if n <= 1:
        return False
    for i in range(2, n):
        if n % i == 0:
            return False
    return True
```

# Functions & Recursion:

### What is a function in Python?
A function is a reusable block of code that performs a specific task.

### How do you define and call a function?
Define a function using the `def` keyword and call it by its name. Example:
```python
def greet():
    print("Hello, World!")
greet()
```

### What is the difference between a built-in function and a user-defined function?
- Built-in function: Provided by Python (e.g., `print()`, `len()`).
- User-defined function: Created by the user to perform specific tasks.

### What are function parameters and arguments?
- Parameters: Variables listed in the function definition.
- Arguments: Values passed to the function when it is called.

### How do you return multiple values from a function?
You can return multiple values as a tuple. Example:
```python
def get_coordinates():
    return (10, 20)
x, y = get_coordinates()
```

### What is recursion? How does it work?
Recursion is a technique where a function calls itself. It works by breaking down a problem into smaller subproblems until a base case is reached.

### What are the advantages and disadvantages of recursion?
- Advantages: Simplifies code, useful for problems like tree traversal and factorial calculation.
- Disadvantages: Can lead to high memory usage and stack overflow if not handled properly.

### How do you calculate factorial using recursion?
```python
def factorial(n):
    if n == 0:
        return 1
    else:
        return n * factorial(n - 1)
```

### How does a recursive function terminate?
A recursive function terminates when it reaches the base case, which does not make further recursive calls.

### How do you find the sum of digits of a number using recursion?
```python
def sum_of_digits(n):
    if n == 0:
        return 0
    else:
        return n % 10 + sum_of_digits(n // 10)
```
# String Manipulation:

### What is string slicing in Python?
String slicing is used to extract a substring from a string. Example:
```python
s = "Hello, World!"
substring = s[0:5]  # Output: 'Hello'
```

### How do you extract every third character from a string?
```python
s = "abcdefg"
result = s[::3]  # Output: 'adg'
```

### What is the difference between `str.upper()` and `str.lower()`?
- `str.upper()`: Converts all characters in the string to uppercase.
- `str.lower()`: Converts all characters in the string to lowercase.

### How do you check if a string contains only digits?
Use the `str.isdigit()` method. Example:
```python
s = "12345"
is_digits = s.isdigit()  # Output: True
```

### How do you reverse a string in Python?
```python
s = "Hello"
reversed_s = s[::-1]  # Output: 'olleH'
```

### What are escape sequences in Python?
Escape sequences are special characters used to represent certain whitespace or non-printable characters. Examples include `\n` (newline), `\t` (tab), and `\\` (backslash).

### How do you check if a character is uppercase, lowercase, a digit, or a special character?
Use methods like `str.isupper()`, `str.islower()`, `str.isdigit()`, and `str.isalnum()`.

### What is the use of `ord()` and `chr()` functions?
- `ord()`: Returns the ASCII value of a character.
- `chr()`: Returns the character corresponding to an ASCII value.

### What is string immutability in Python?
String immutability means that once a string is created, its content cannot be changed. Any operation that modifies a string will create a new string.

### How do you count vowels in a given string?
```python
s = "Hello, World!"
vowels = "aeiouAEIOU"
count = sum(1 for char in s if char in vowels)
```

# Lists, Tuples, Sets, and Dictionaries:

### What is the difference between lists and tuples?
- Lists: Mutable, can be changed after creation.
- Tuples: Immutable, cannot be changed after creation.

### How do you create a list in Python?
```python
my_list = [1, 2, 3, 4, 5]
```

### How do you add and remove elements from a list?
- Add: `list.append()`, `list.insert()`, `list.extend()`
- Remove: `list.remove()`, `list.pop()`, `del`

### How do you find the largest and second-largest element in a list?
```python
my_list = [1, 3, 4, 5, 0, 2]
largest = max(my_list)
my_list.remove(largest)
second_largest = max(my_list)
```

### What is list comprehension?
List comprehension is a concise way to create lists using a single line of code. Example:
```python
squares = [x**2 for x in range(10)]
```

### How do you remove duplicates from a list?
Convert the list to a set and back to a list. Example:
```python
my_list = [1, 2, 2, 3, 4, 4, 5]
my_list = list(set(my_list))
```

### What is a tuple, and how is it different from a list?
A tuple is an immutable sequence of elements. It is different from a list in that it cannot be changed after creation.

### How do you create a set in Python?
```python
my_set = {1, 2, 3, 4, 5}
```

### How do you perform set operations like union, intersection, and difference?
- Union: `set1.union(set2)` or `set1 | set2`
- Intersection: `set1.intersection(set2)` or `set1 & set2`
- Difference: `set1.difference(set2)` or `set1 - set2`

### How do you update a set with elements that are not in another set?
Use the `difference_update()` method. Example:
```python
set1 = {1, 2, 3, 4}
set2 = {3, 4, 5, 6}
set1.difference_update(set2)  # set1 becomes {1, 2}
```

### What is a dictionary in Python?
A dictionary is a collection of key-value pairs, where each key is unique. Example:
```python
my_dict = {"name": "Alice", "age": 30}
```

### How do you access dictionary keys and values?
- Access keys: `dict.keys()`
- Access values: `dict.values()`

### How do you merge two dictionaries?
Use the `update()` method. Example:
```python
dict1 = {"name": "Alice"}
dict2 = {"age": 30}
dict1.update(dict2)  # dict1 becomes {"name": "Alice", "age": 30}
```

### How do you sort a dictionary by its keys or values?
- Sort by keys: `sorted(dict.items())`
- Sort by values: `sorted(dict.items(), key=lambda item: item[1])`

### How do you check if a key exists in a dictionary?
Use the `in` keyword. Example:
```python
if "name" in my_dict:
    print("Key exists")
```

# Mathematical & Logical Computations:

### How do you calculate the area of a circle in Python?
```python
import math
radius = 5
area = math.pi * (radius ** 2)
```

### How do you convert kilometers to miles?
```python
km = 5
miles = km * 0.621371
```

### How do you check if a year is a leap year?
```python
def is_leap_year(year):
    if (year % 4 == 0 and year % 100 != 0) or (year % 400 == 0):
        return True
    return False
```

### What is the difference between `//` and `%` operators?
- `//`: Integer division, returns the quotient.
- `%`: Modulus operator, returns the remainder.

### How do you find the maximum of three numbers using `if-else`?
```python
a, b, c = 10, 20, 30
if a > b and a > c:
    max_num = a
elif b > a and b > c:
    max_num = b
else:
    max_num = c
```

### How do you find the sum of the first `n` natural numbers?
```python
n = 10
sum = n * (n + 1) // 2
```

### How do you generate a random number in Python?
```python
import random
random_number = random.randint(1, 100)
```

### How do you find the factorial of a number using iteration?
```python
def factorial(n):
    result = 1
    for i in range(1, n + 1):
        result *= i
    return result
```

### What is the significance of the `math` module in Python?
The `math` module provides mathematical functions and constants, such as `math.sqrt()`, `math.pi`, `math.sin()`, etc.

### How do you calculate the angle of the hour hand of a clock?
```python
def hour_angle(hour, minutes):
    angle = (hour % 12) * 30 + minutes * 0.5
    return angle
```

# File Handling & Exception Handling (If Covered):

### What is file handling in Python?
File handling is the process of opening, reading, writing, and closing files in Python.

### How do you open and close a file in Python?
Use the `open()` function to open a file and the `close()` method to close it. Example:
```python
file = open("example.txt", "r")
file.close()
```

### What are the different file modes in Python?
- `r`: Read mode
- `w`: Write mode
- `a`: Append mode
- `b`: Binary mode

### How do you read and write files in Python?
- Read: `file.read()`, `file.readline()`, `file.readlines()`
- Write: `file.write()`, `file.writelines()`

### What are exceptions in Python?
Exceptions are errors that occur during the execution of a program, which can be handled using try-except blocks.

### How do you handle exceptions using try-except blocks?
```python
try:
    # code that may raise an exception
    pass
except Exception as e:
    # code to handle the exception
    print(e)
```

### What is the difference between finally and else in exception handling?
- `finally`: Block of code that always executes, regardless of whether an exception occurred.
- `else`: Block of code that executes if no exception occurred.

# Miscellaneous & Advanced Concepts:

### What is the difference between `is` and `==` in Python?
- `is`: Checks if two variables refer to the same object in memory.
- `==`: Checks if the values of two variables are equal.

### What are lambda functions?
Lambda functions are anonymous functions defined using the `lambda` keyword. Example:
```python
add = lambda x, y: x + y
print(add(2, 3))  # Output: 5
```

### What is the purpose of `zip()` in Python?
The `zip()` function combines elements from multiple iterables into tuples. Example:
```python
list1 = [1, 2, 3]
list2 = ['a', 'b', 'c']
zipped = zip(list1, list2)
print(list(zipped))  # Output: [(1, 'a'), (2, 'b'), (3, 'c')]
```

### How do you use `map()` and `filter()` functions?
- `map()`: Applies a function to all items in an iterable.
- `filter()`: Filters items in an iterable based on a function.

Example:
```python
numbers = [1, 2, 3, 4, 5]
squared = map(lambda x: x**2, numbers)
evens = filter(lambda x: x % 2 == 0, numbers)
print(list(squared))  # Output: [1, 4, 9, 16, 25]
print(list(evens))    # Output: [2, 4]
```

### What is a decorator in Python?
A decorator is a function that takes another function and extends its behavior without explicitly modifying it. Example:
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

### What is the purpose of the `random` module?
The `random` module provides functions for generating random numbers. Example:
```python
import random
print(random.randint(1, 10))  # Output: Random number between 1 and 10
```

### How do you implement a password validation function in Python?
```python
import re

def validate_password(password):
    if len(password) < 8:
        return False
    if not re.search("[a-z]", password):
        return False
    if not re.search("[A-Z]", password):
        return False
    if not re.search("[0-9]", password):
        return False
    if not re.search("[@#$]", password):
        return False
    return True

password = "Password123@"
print(validate_password(password))  # Output: True
```

### How do you check if a given sequence of numbers is a palindrome?
```python
def is_palindrome(sequence):
    return sequence == sequence[::-1]

sequence = [1, 2, 3, 2, 1]
print(is_palindrome(sequence))  # Output: True
```

### What is the difference between mutable and immutable data types?
- Mutable: Can be changed after creation (e.g., list, dict, set).
- Immutable: Cannot be changed after creation (e.g., int, float, str, tuple).

### How do you check if two sets have common elements?
```python
set1 = {1, 2, 3}
set2 = {3, 4, 5}
common = set1 & set2  # Intersection
print(bool(common))   # Output: True
```

### How do you print Fibonacci numbers using recursion?
```python
def fibonacci(n):
    if n <= 0:
        return []
    elif n == 1:
        return [0]
    elif n == 2:
        return [0, 1]
    else:
        fibs = fibonacci(n - 1)
        fibs.append(fibs[-1] + fibs[-2])
        return fibs

print(fibonacci(10))  # Output: [0, 1, 1, 2, 3, 5, 8, 13, 21, 34]
```

### What is memoization, and how can it optimize recursive calls?
Memoization is a technique for optimizing recursive calls by caching the results of expensive function calls and reusing them when the same inputs occur again. Example:
```python
def memoize(f):
    cache = {}
    def memoized_function(*args):
        if args not in cache:
            cache[args] = f(*args)
        return cache[args]
    return memoized_function

@memoize
def fibonacci(n):
    if n in {0, 1}:
        return n
    return fibonacci(n - 1) + fibonacci(n - 2)

print([fibonacci(x) for x in range(10)])  # Output: [0, 1, 1, 2, 3, 5, 8, 13, 21, 34]
```

### What is the difference between shallow copy and deep copy?
- Shallow copy: Creates a new object but inserts references into it to the objects found in the original.
- Deep copy: Creates a new object and recursively copies all objects found in the original.

Example:
```python
import copy

original = [[1, 2, 3], [4, 5, 6]]
shallow = copy.copy(original)
deep = copy.deepcopy(original)

original[0][0] = 10
print(shallow)  # Output: [[10, 2, 3], [4, 5, 6]]
print(deep)     # Output: [[1, 2, 3], [4, 5, 6]]
```

### How do you use `sorted()` with custom sorting criteria?
You can use the `key` parameter to specify a custom sorting function. Example:
```python
students = [("Alice", 25), ("Bob", 20), ("Charlie", 23)]
sorted_students = sorted(students, key=lambda x: x[1])
print(sorted_students)  # Output: [('Bob', 20), ('Charlie', 23), ('Alice', 25)]
```

### How do you check if a date is valid?
```python
from datetime import datetime

def is_valid_date(date_str):
    try:
        datetime.strptime(date_str, "%Y-%m-%d")
        return True
    except ValueError:
        return False

print(is_valid_date("2025-02-19"))  # Output: True
print(is_valid_date("2025-02-30"))  # Output: False
```

### What is the purpose of `difference_update()` in sets?
The `difference_update()` method removes all elements of another set from the original set. Example:
```python
set1 = {1, 2, 3, 4}
set2 = {3, 4, 5, 6}
set1.difference_update(set2)
print(set1)  # Output: {1, 2}
```

### How do you implement ASCII character mapping in Python?
Use the `ord()` and `chr()` functions for ASCII character mapping. Example:
```python
char = 'A'
ascii_value = ord(char)
print(ascii_value)  # Output: 65

ascii_value = 97
char = chr(ascii_value)
print(char)  # Output: 'a'
```

### What is the significance of the `@staticmethod` and `@classmethod` decorators?
- `@staticmethod`: Defines a method that does not operate on an instance or class.
- `@classmethod`: Defines a method that takes the class as the first parameter.

Example:
```python
class MyClass:
    @staticmethod
    def static_method():
        print("This is a static method")

    @classmethod
    def class_method(cls):
        print("This is a class method")

MyClass.static_method()  # Output: This is a static method
MyClass.class_method()   # Output: This is a class method
```
```` ▋
