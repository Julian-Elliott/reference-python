# Python Cheat Sheets

## Quick Reference

### Variables and Data Types
```python
# Numbers
age = 25
height = 5.9
is_student = True

# Strings
name = "Python Champion"
greeting = f"Hello, {name}!"

# Lists
lucky_numbers = [7, 13, 21, 42]
mixed_list = [1, "hello", True, 3.14]

# Dictionaries
person = {
    "name": "Lucky Coder",
    "score": 100,
    "streak": "ongoing"
}
```

### Control Flow
```python
# If statements
if score >= 90:
    print("Excellent! Another lucky day!")
elif score >= 80:
    print("Good job!")
else:
    print("Keep practicing!")

# Loops
for number in lucky_numbers:
    print(f"Lucky number: {number}")

# While loop
attempts = 0
while attempts < 3:
    print(f"Attempt {attempts + 1}")
    attempts += 1
```

### Functions
```python
def calculate_luck_factor(preparation, opportunity):
    """Where preparation meets opportunity"""
    return preparation * opportunity

def get_quiz_strategy():
    return [
        "Read carefully",
        "Think before answering", 
        "Trust your preparation",
        "Stay confident"
    ]
```

### Common Patterns
```python
# List comprehensions
even_numbers = [x for x in range(20) if x % 2 == 0]
squared = [x**2 for x in range(10)]

# Dictionary comprehensions
word_lengths = {word: len(word) for word in ["python", "coding", "lucky"]}

# Error handling
try:
    result = risky_operation()
except Exception as e:
    print(f"Handled gracefully: {e}")
finally:
    print("Always executes")
```

### Advanced Tips
- Use `enumerate()` for index and value
- `zip()` for parallel iteration
- `*args` and `**kwargs` for flexible functions
- List slicing: `lst[start:end:step]`
- String methods: `.strip()`, `.split()`, `.join()`
