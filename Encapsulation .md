# 🐍 Python OOP: Encapsulation with Private Members

## 🎯 AIM

To implement **Encapsulation** in Python by defining a class `Rectangle` with **private member variables** `__length` and `__breadth`.

---

## 🧠 ALGORITHM

1. **Define the Class**:
   - Create a class `Rectangle` with two private attributes: `__length` and `__breadth`.

2. **Initialize Variables**:
   - Use the `__init__()` constructor to set initial values for `__length` and `__breadth`.

3. **Print Values**:
   - Display the private variables from within the class to demonstrate access.

4. **Instantiate the Object**:
   - Create an object of the `Rectangle` class to trigger the constructor.

---

## 💻 Program
class Rectangle: def init(self, length, breadth): self.__length = length # private variable self.__breadth = breadth # private variable

def calculate_area(self):
    return self.__length * self.__breadth

def get_length(self):
    return self.__length

def get_breadth(self):
    return self.__breadth
l = int(input("Enter length: ")) b = int(input("Enter breadth: "))

rect = Rectangle(l, b)

print("Length:", rect.get_length()) print("Breadth:", rect.get_breadth()) print("Area of Rectangle:", rect.calculate_area())

## Output
Enter length: 5 Enter breadth: 3 Length: 5 Breadth: 3 Area of Rectangle: 15

## Result
The program executed successfully and demonstrated encapsulation in Python by using private variables __length and __breadth and accessing them through methods.
