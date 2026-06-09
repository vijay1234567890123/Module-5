# # Constructors in Python: Welcome Message with Student Name

## 🎯 Aim
To write a Python program that creates a **Student** class with a **default constructor** and a method to display a welcome message along with the student’s name provided by the user.

## 🧠 Algorithm
1. **Get user input**: Accept the student's name from the user.
2. **Define the class**: Create a class `Student` with a default constructor (`__init__`).
3. **Default Constructor**: In the constructor, assign the user input (student name) to an instance variable `self.a`.
4. **Display Message**: Define a method `show` that prints "This is non-parameterized constructor" and a welcome message with the student’s name.
5. **Execute the Program**: Instantiate the `Student` class and call the `show` method.

## 🧾 Program
```
name = input("Enter the student's name: ")

class Student:
   
    def __init__(self):
        self.a = name  # assign user input to instance variable

    def show(self):
        print("This is a non-parameterized constructor")
        print("Welcome,", self.a)

s = Student()
s.show()
```

## Output
<img width="530" height="152" alt="image" src="https://github.com/user-attachments/assets/30e8d348-56b8-4693-8790-54c8904af1fd" />

## Result
Thus , To write a Python program that creates a Student class with a default constructor and a method to display a welcome message along with the student’s name provided by the user.
