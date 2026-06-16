# Python Syntax - Complete Beginner Notes

## 1. What is Python Syntax?

Syntax means the **rules** that Python follows to understand your code. Just like English has grammar rules, Python has syntax rules. If you break them, Python will throw an error and refuse to run your code.

---

## 2. The `print()` Function - Your First Tool

`print()` is a built-in function in Python that displays (prints) whatever you give it on the screen.

### How it works:

```python
print("Hello World!")
```

**Breaking it down:**

| Part | Meaning |
|------|---------|
| `print` | Name of the function |
| `(` | Opening parenthesis - tells Python "here comes the input" |
| `"Hello World!"` | The argument (input) - what you want to print |
| `)` | Closing parenthesis - tells Python "input is done" |

### Key Points:
- `print` is the **function name**
- Parentheses `()` are used to **call** (execute) the function
- Whatever you put inside `()` is called an **argument**
- The function processes the argument and shows output on screen

---

## 3. What is a Function?

A function is a **reusable block of code** that performs a specific task.

- `print()` → prints things on screen
- `abs()` → returns the absolute value of a number

```python
print("Hello")    # prints: Hello
abs(-5)           # returns: 5
```

Different functions do different things. You can even write your own custom functions (covered in later topics).

---

## 4. Python Executes Code Line by Line (Top to Bottom)

Python reads your file from **top to bottom** and executes each line one by one, in order.

### Example:

```python
print("Hello Harry")
print("I am good")
print("How are you?")
```

### Output:

```
Hello Harry
I am good
How are you?
```

**What happened?**
- Line 1 → Python prints "Hello Harry"
- Line 2 → Python prints "I am good"
- Line 3 → Python prints "How are you?"

Each `print()` automatically adds a **new line** at the end, so the next output appears on the next line.

---

## 5. Strings and Numbers in `print()`

### Strings (Text):
Anything written inside **double quotes** `" "` or **single quotes** `' '` is called a **string**.

```python
print("Hello Harry")   # This is a string
print('I am good')     # This is also a string
```

### Numbers:
You can also pass numbers directly (without quotes).

```python
print(3)    # prints: 3
print(100)  # prints: 100
```

---

## 6. How to Run a Python Program

There are two common ways to run a Python file:

### Method 1: Using Terminal
```
python main.py
```

### Method 2: Using the Run button in VS Code
Click the ▶️ (play) icon in VS Code.

### Tip:
Press the **Up Arrow** key in terminal to repeat the last command you typed. This saves time when running the same file again.

---

## 7. Syntax Errors - What Happens When You Write Wrong Code

If you write something Python doesn't understand, it throws a **SyntaxError**.

### Example:

```python
print("Hello Harry")
print("I am good")
print("How are you?")
asdkjfhaskjdfh          # This is gibberish - Python can't understand it
```

### What happens:

```
SyntaxError: invalid syntax
```

### Key Points about Syntax Errors:
- Python **scans the entire file first** before running anything
- If it finds a syntax error, **none of the lines execute** — not even the correct ones
- Python tells you the **exact line number** where the error is
- VS Code also shows a **red underline** warning before you even run the code
- You must **fix the error** before running the program again

---

## 8. Indentation - Python's Way of Organizing Code

Indentation means adding **spaces at the beginning of a line**. In Python, indentation is **not optional** — it is part of the syntax.

### What is Indentation?

Indentation tells Python which lines of code belong **inside** a block (like an `if` statement, loop, or function).

### Example:

```python
if a > 3:
    print("Inside the if block")     # This is INSIDE (has 4 spaces)
    print("Also inside")             # This is INSIDE (has 4 spaces)
print("Outside the if block")        # This is OUTSIDE (no spaces)
```

### Visual Explanation:

```
if a > 3:
    ┊  statement 1    ← INSIDE the if block (indented)
    ┊  statement 2    ← INSIDE the if block (indented)
statement 3           ← OUTSIDE the if block (no indentation)
```

### Key Points:
- Python uses **4 spaces** (or 1 tab) for indentation
- Indentation tells Python what is **inside** a block and what is **outside**
- Wrong indentation = Error
- VS Code automatically adds indentation when you press Enter after a colon `:`

> **Note:** We will learn `if` statements and loops in detail later. For now, just understand that indentation = spaces that show code belongs inside a block.

---

## 9. Comments - Hiding Code from Python

A **comment** is a line that Python completely ignores. It is written for humans, not for the computer.

### How to write a comment:

Put a `#` (hashtag) at the beginning of the line.

```python
# This is a comment - Python ignores this
print("Hello")   # This part after # is also a comment
```

### Why use comments?

1. **To explain your code** to yourself or others
2. **To temporarily disable code** without deleting it

### Example - Disabling code:

```python
print("Hello Harry")
print("I am good")
print("How are you?")
print(3)
# if a > 3:
#     print("statement 1")
#     print("statement 2")
# print("statement 3")
```

Now lines 5-8 are **ignored** by Python. The program runs without errors.

### VS Code Shortcut:
- Select lines → Press `Ctrl + /` → Toggles comments on/off

---

## 10. Quick Summary

| Concept | What It Means |
|---------|---------------|
| `print()` | Function that displays output on screen |
| Function | Reusable code that does a specific task |
| Argument | The value you pass inside `()` to a function |
| String | Text inside quotes (`"hello"` or `'hello'`) |
| Line-by-line execution | Python runs code from top to bottom, one line at a time |
| SyntaxError | Python can't understand your code - fix it before running |
| Indentation | Spaces at the start of a line to show code is inside a block |
| Comment (`#`) | Line ignored by Python, used for notes or disabling code |

---

## 11. Practice Exercise

Try writing this in a `main.py` file and run it:

```python
# My first Python program
print("My name is Arbind")
print("I am learning Python")
print("Python is fun!")
print(2025)

# The line below is commented out - Python will skip it
# print("This will NOT be printed")
```

### Expected Output:

```
My name is Arbind
I am learning Python
Python is fun!
2025
```

---

## What's Coming Next?

In the upcoming topics, we will learn:
- Variables
- Data Types
- User Input in Python

---

> **Remember:** Don't worry if everything doesn't click immediately. As you practice more, Python syntax will become natural to you. Just keep writing code!
