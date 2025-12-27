# Multilevel Inheritance Example in Python

This Python project demonstrates the concept of **Multilevel Inheritance** to collect and display the **name**, **age**, and **location** of a person.

## 🎯 Aim

To write a Python program that uses multilevel inheritance to get and display a person’s name, age, and location.

## 🧠 Algorithm

1. **Parent Class**  
   - `__init__(name)` initializes the `name` attribute.  
   - `getName()` returns the `name`.

2. **Child Class (inherits Parent)**  
   - `__init__(name, age)` initializes `name` using `super()` and adds `age`.  
   - `getAge()` returns the `age`.

3. **Grandchild Class (inherits Child)**  
   - `__init__(name, age, location)` initializes `name` and `age` using `super()` and adds `location`.  
   - `getLocation()` returns the `location`.

4. **Input & Output**  
   - Take user input for name, age, and location.  
   - Create an instance of `Grandchild`.  
   - Print all details using class methods.

## Program
```
# Base class
class Person:
    def __init__(self, name):
        self.name = name

# Derived class (Level 2)
class Age(Person):
    def __init__(self, name, age):
        super().__init__(name)
        self.age = age

# Derived class (Level 3)
class Location(Age):
    def __init__(self, name, age, location):
        super().__init__(name, age)
        self.location = location

    def display(self):
        print("Name:", self.name)
        print("Age:", self.age)
        print("Location:", self.location)


# Object creation and input
name = input("Enter name: ")
age = int(input("Enter age: "))
location = input("Enter location: ")

obj = Location(name, age, location)
obj.display()
```

## Sample Output
<img width="930" height="815" alt="image" src="https://github.com/user-attachments/assets/b57b0d2a-8cc1-4c90-9e33-086782f355d5" />

