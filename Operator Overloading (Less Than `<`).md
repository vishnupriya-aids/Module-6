# 🐍 Python OOP: Operator Overloading (Less Than `<`)

## 🎯 AIM

To write a Python program that demonstrates **operator overloading** by overloading the **less than (`<`)** operator using a custom class.

---

## 🧠 ALGORITHM

1. **Create Class `A`**:
   - Define the `__init__()` method to initialize the object with a value `a`.

2. **Overload the `<` Operator**:
   - Define the `__lt__()` method with logic:
     - If `self.a < o.a`, return `"ob1 is less than ob2"`
     - Else, return `"ob2 is less than ob1"`

3. **Create Objects**:
   - Instantiate two objects `ob1` and `ob2` with values.

4. **Use `<` Operator**:
   - Use `print(ob1 < ob2)` to trigger the overloaded behavior.

---

## 💻 Program

class Number: def init(self, value): self.value = value

def __lt__(self, other):
    return self.value < other.value
a = int(input("Enter first number: ")) b = int(input("Enter second number: "))

num1 = Number(a) num2 = Number(b) if num1 < num2: print(a, "is less than", b) else: print(a, "is not less than", b)
## Output
Enter first number: 10 Enter second number: 20 10 is less than 20

## Result
The program executed successfully and demonstrated operator overloading by redefining the < operator using the lt method in a custom class.
