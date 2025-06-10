# Notes and Jot: Objects

---

In Python, **everything is an object**—from simple values like numbers and strings to complex constructs like functions and modules. Understanding objects is key to mastering Python’s flexibility and power. Let’s break it down step by step.

## 1. What Is an Object?
- **Every value** you work with is an object in memory.
- An object bundles together:
    1. **Data** (its attributes or state)
    2. **Behavior** (its methods or functions you can call on it)

> **Analogy:** Think of an object like a **smart appliance** (e.g., a smart speaker). It has:
> - A **state** (volume level, Wi-Fi connected or not)     
> - **Actions** you can ask it to perform (play music, tell the weather).

---
## 2. How Objects Work “Under the Hood”
1. **Creation**
    - When you write `x = 10`, Python:
        - Allocates memory for an integer object with the value `10`.
        - Binds the name `x` to that object.         
2. **Identity, Type, and Value**
    - **Identity**: Each object has a unique ID (you can see it with `id(obj)`), like a street address.
    - **Type**: Determines which operations are allowed and which methods exist (you can check with `type(obj)`).
    - **Value**: The actual data stored (e.g., `10` for an integer).
3. **Reference Counting & Garbage Collection**
    - Python keeps track of how many names point to each object.
    - When no references remain, Python frees the memory automatically.

---

## 3. Creating Your Objects: Classes & Instances
Python lets you define custom object types with `class` A class is like a blueprint; an `instance` is a concrete object built from that blueprint.
```python
class Dog:
    def __init__(self, name, age):
        # Attributes (state)
        self.name = name
        self.age = age

    # Method (behavior)
    def bark(self):
        print(f"{self.name} says: Woof!")

# Create (instantiate) two Dog objects
fido = Dog("Fido", 3)
luna = Dog("Luna", 1)

fido.bark()  # Output: Fido says: Woof!
luna.bark()  # Output: Luna says: Woof!
```
- `class Dog:` defines a new object **type** named `Dog`.
- `__init__` is the **constructor**: it runs when you do `Dog(...)`.
- `self` refers to the particular instance being created.
- `fido` and `luna` are two **instances** (objects) of type `Dog`.

---

## 4. Attributes vs. Methods
- **Attributes** store data. You access them as `object.attribute`.
- **Methods** are functions defined on the class; you call them as `object.method()`.
```python
print(fido.name)   # Attribute access: "Fido" fido.age = 4       # You can change attributes at runtime print(fido.age)    # Now 4
```


---

## 5. Python’s Built-In Objects
Python comes with many ready-to-use object types:

| Category      | Examples                                             | Use Case                             |
| ------------- | ---------------------------------------------------- | ------------------------------------ |
| **Numbers**   | `int`, `float`, `complex`                            | Counting, measurements, calculations |
| **Sequences** | `str`, `list`, `tuple`, `range`                      | Ordered collections, text processing |
| **Mappings**  | `dict`                                               | Key–value stores                     |
| **Sets**      | `set`, `frozenset`                                   | Unordered unique collections         |
| **Files**     | `open` returns a file object                         | Reading/writing files                |
| **Functions** | Any function (`def` or `lambda`) is itself an object | First-class functions, decorators    |
| **Modules**   | Everything you `import`                              | Namespaces grouping code             |

**Example: Working with built-ins**
```python
# List (sequence)
fruits = ["apple", "banana", "cherry"]
fruits.append("date")          # Method call
print(fruits[1])               # Indexing: "banana"

# Dictionary (mapping)
prices = {"apple": 0.40, "banana": 0.25}
prices["cherry"] = 0.60        # Add/update entry
print(prices.get("date", 0))   # Safely get with default: 0

# String (immutable sequence)
name = "Alice"
print(name.upper())            # Method: "ALICE"

```


---

## 6. Why Use Objects?
1. **Organization**: Group related data and behavior together.
2. **Reusability**: Define general blueprints (classes) and reuse them.
3. **Encapsulation**: Hide internal details—only expose what you need via methods.
4. **Polymorphism**: Different object types can provide the same method names and be used interchangeably (e.g., both lists and strings support `len()`).

---

## 7. Key Takeaways

- **Object** = data + behavior, stored in memory with an identity, type, and value.
- **Everything** in Python is an object, including functions and modules.
- You create custom objects via `class` and instantiate them by calling the class.
- Python’s built-in objects (numbers, strings, lists, dicts, etc.) give you powerful tools out of the box.