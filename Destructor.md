# Exp.No:22  
## Destructor

---

### AIM  
To create a Python class `Student` with a destructor.

---

### ALGORITHM

1. Begin the program.  
2. Define the `student` class.  
3. Inside the `student` class, define the `__init__` method (constructor) and the `__del__` method (destructor).  
4. Create an object `s2` of the `student` class. When the object `s2` is created, the `__init__` method is called, and its print statements are executed.  
5. Use the `del` statement to delete the object `s2`. This triggers the `__del__` method (destructor), and the respective print statements are executed.  
6. Terminate the program.

---

### PROGRAM

```
class Student:
    def __init__(self):
        print("Constructor: Student object is created.")
    def __del__(self):
        print("Destructor: Student object is destroyed.")

s2 = Student()

del s2

```

### OUTPUT

![image](https://github.com/user-attachments/assets/078aae07-6a4d-4565-a985-2b524f22f99d)

### RESULT

Thus, the program to create a Python class `Student` with a destructor has been executed and verified successfully.
