# Destructor in Python

This project demonstrates how to implement a **destructor** in Python using a simple class.

## 🚀 Overview

The program defines a class `Demo` with:

- A **constructor** `__init__` that initializes an instance variable and prints a message.
- A **destructor** `__del__` that prints a message when the object is destroyed.

## 🧠 Algorithm

1. Define a class named `Demo`.
2. Inside the class, define the `__init__` method:
   - Initialize an instance variable `status` with the value `"Alive"`.
   - Print the value of `status`.
3. Define the `__del__` method:
   - Print a message indicating the object is being destroyed.
4. Outside the class:
   - Create an instance of the `Demo` class.
   - Delete the object using the `del` keyword.
## Program
```
class Demo:
    def __init__(self):
        self.value = 10
        print("Constructor called: Object created")

    def __del__(self):
        print("Destructor called: Object destroyed")

# Creating object
obj = Demo()

# Deleting object explicitly (optional)
del obj
```

## 🧪 Output
<img width="533" height="711" alt="image" src="https://github.com/user-attachments/assets/9f416a04-4925-4f78-adfb-ee6a09203080" />

## Result

