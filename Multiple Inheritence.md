# Arithmetic Operations Using Multiple Inheritance in Python

This Python program demonstrates **multiple inheritance** by performing basic arithmetic operations — Addition, Subtraction, and Division — using three classes.

## 🎯 Aim

To write a Python program to calculate **Add, Sub & Division** using **Multiple Inheritance**.

## 🧠 Algorithm

1. **Define `Calculation1` class**
   - Contains `Summation(a, b)` method to return the sum of two numbers.
2. **Define `Calculation2` class**
   - Contains `Subtraction(a, b)` method to return the difference of two numbers.
3. **Define `Derived` class**
   - Inherits from both `Calculation1` and `Calculation2`.
   - Contains `Division(a, b)` method to return the division result.
4. **Input**
   - Prompt the user to enter two numbers.
5. **Process**
   - Create an object of the `Derived` class.
   - Call `Summation`, `Subtraction`, and `Division` methods.
6. **Output**
   - Display the results of the three operations.

## 💻 Program 
```
# Parent class 1
class Add:
    def add(self, a, b):
        return a + b

# Parent class 2
class Sub:
    def sub(self, a, b):
        return a - b

# Child class (inherits from Add and Sub)
class Calc(Add, Sub):
    def div(self, a, b):
        return a / b


# Input
a = int(input("Enter first number: "))
b = int(input("Enter second number: "))

# Object creation
c = Calc()

# Output
print("Addition:", c.add(a, b))
print("Subtraction:", c.sub(a, b))
print("Division:", c.div(a, b))
```
## Output Example

<img width="930" height="815" alt="image" src="https://github.com/user-attachments/assets/de3e383f-cfe2-405d-99cd-d756a4c7e7fd" />
