---
title: "Intro to Python"
---

## Intro

This guide is designed as a quick-reference for Python fundamentals.

## 1. Strings

Strings can be defined with single, double, or triple quotes.

```python
print("Hello, world!")
print('Hello, world!')
print("""This is a
multiple line string!""")
print("This string is " + "Awesome") # Concatenation
```

## 2. Math Operations

Python follows standard mathematical order (PEMDAS).

```python
print(50 + 50)   # Add
print(50 - 50)   # Subtract
print(50 * 50)   # Multiply
print(50 / 50)   # Divide
print(50 ** 2)   # Exponents (50 squared)
print(50 % 6)    # Modulus (Remainder)
print(50 // 6)   # Floor Division (Drops decimals)
```

## 3. Variables & Methods

Variables are used to store data. Methods are functions that belong to an object.

```python
name = "Hanif"    # String
age = 18          # Int
gpa = 3.7         # Float

quote = "Cinta itu buta"
print(quote.upper()) # UPPERCASE
print(quote.lower()) # lowercase
print(len(quote))    # Length of string

# Type conversion (Casting)
print("My name is " + name + " and I am " + str(age) + " years old.")
```

## 4. Functions

Functions are reusable blocks of code.

```python
def who_am_i():
    name = "Hanif"
    print("I am " + name)

who_am_i() # Calling function

def multiply(x, y):
    return x * y # Returns value to the caller

print(multiply(7, 7))
```

## 5. Boolean & Relational Operators

Used for logic and comparisons.

```python
bool1 = True
bool2 = (3 * 3 == 9)           # True
test_and = (7 > 5) and (5 < 7) # True
test_or = (7 > 5) or (10 < 2)  # True
test_not = not True            # False
```

## 6. Conditional Statements

Control the flow of your program based on conditions.

```python
def smoking(age, money):
    if (age >= 21) and (money >= 5):
        return "Yes, go smoking"
    elif (age >= 21) and (money < 5):
        return "No money"
    elif (age < 21):
        return "Too young / Haram"
    else:
        return "No money and young"

print(smoking(21, 5))
```

## 7. Lists & Tuples

**Lists** are ordered and can be changed. **Tuples** are ordered but cannot be changed.

```python
# Lists []
movies = ["Inception", "Interstellar", "Batman"]
print(movies[0])      # First item
movies.append("New")  # Add item
movies.pop()          # Remove last item

# Tuples ()
grades = ("A", "B", "C")
```

## 8. Looping

Use loops to repeat tasks.

```python
# For Loop (Iterating over a list)
vegetables = ["cucumber", "spinach", "cabbage"]
for x in vegetables:
    print(x)

# While Loop (Executing while a condition is true)
i = 1
while i < 10:
    print(i)
    i += 1
```

## 9. Advanced Strings & Formatting

```python
sentence = "This is a sentence."
print(sentence.split()) # ['This', 'is', 'a', 'sentence.']

# F-Strings (The modern way to format)
movie = "Mr Robot"
print(f"My favorite movie is {movie}.")
```

## 10. Dictionaries

Key-value pairs, similar to a real-life dictionary.

```python
drinks = {"sirap": 2, "oren": 3, "kosong": 1}
print(drinks["sirap"]) # Returns 2
```

## 11. Sockets (Networking)

Sockets allow you to connect nodes together over a network.

```python
import socket

HOST = '127.0.0.1'
PORT = 7777

# Create a socket object (IPv4, TCP)
s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
s.connect((HOST, PORT))
```

## 12. File Handling

How to read from and write to files.

```python
# Writing to a file (will overwrite existing)
with open("test.txt", "w") as f:
    f.write("Hello from 0xhanif!")

# Appending to a file
with open("test.txt", "a") as f:
    f.write("\nAdding a new line.")

# Reading a file
with open("test.txt", "r") as f:
    print(f.read())
```

## 13. Classes & Objects

Object-Oriented Programming (OOP) allows you to create your own data types.

```python
class Cat:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def meow(self):
        print("Meow!")

    def display_info(self):
        print("Name:", self.name)
        print("Age:", self.age)

# Create Object
cat1 = Cat("Oyen", 5)
cat2 = Cat("Puteh", 3)
cat1.meow()             # Output: "Meow!"
cat1.display_info()     # Output: "Name: Oyen", "Age: 5"
```

## 14. Pro-tip

In Python, indentation (spaces) is part of the syntax. If your code is not aligned correctly, it will throw an IndentationError.

## Reference

- <https://www.w3schools.com/python/default.asp>
- <https://www.python.org/>
