# 🐍 Python OOP: Abstract Class & Method Example

## 🎯 AIM

To create an **abstract class** named `Shape` with an **abstract method** `calculate_area`, and implement this method in two subclasses: `Rectangle` and `Circle`.

---

## 🧠 ALGORITHM

1. **Import ABC module**:
   - Use `from abc import ABC, abstractmethod` to define abstract classes and methods.

2. **Create Abstract Class `Shape`**:
   - Define an abstract method `calculate_area()` with `@abstractmethod`.

3. **Create Subclass `Rectangle`**:
   - Set default values for `length` and `breadth`.
   - Override `calculate_area()` to compute the rectangle area.

4. **Create Subclass `Circle`**:
   - Set default value for `radius`.
   - Override `calculate_area()` to compute the circle area.

5. **Create Objects & Call Methods**:
   - Instantiate `Rectangle` and `Circle`.
   - Call their `calculate_area()` methods.

---

## 💻 Program

from abc import ABC, abstractmethod class Shape(ABC):

@abstractmethod
def calculate_area(self):
    pass
class Rectangle(Shape): def init(self, length, breadth): self.length = length self.breadth = breadth

def calculate_area(self):
    return self.length * self.breadth
class Circle(Shape): def init(self, radius): self.radius = radius

def calculate_area(self):
    return 3.14 * self.radius * self.radius
l = float(input("Enter length of rectangle: ")) b = float(input("Enter breadth of rectangle: ")) rect = Rectangle(l, b) r = float(input("Enter radius of circle: ")) circle = Circle(r) print("Area of Rectangle:", rect.calculate_area()) print("Area of Circle:", circle.calculate_area())
## Output

Enter length of rectangle: 5 Enter breadth of rectangle: 4 Enter radius of circle: 3 Area of Rectangle: 20.0 Area of Circle: 28.26
## Result

The program executed successfully and demonstrated abstraction by defining an abstract class Shape with an abstract method calculate_area, which was implemented in Rectangle and Circle subclasses.
