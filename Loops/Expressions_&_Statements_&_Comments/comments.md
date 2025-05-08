## **Comments in Python**

Welcome! In this presentation, we will learn about **comments in Python**—what they are, how to use them, and why they are important.
Let’s take a look at the topics we’ll cover:

### **Topics Covered**

1. Introduction to Comments
2. Single-Line Comments
3. Multi-Line Comments
4. Uses of Comments

---

### **1. Introduction to Comments**

A **comment** is a piece of text in a program that is **ignored by the Python interpreter**.
Its purpose is to **improve the readability of the code** by providing explanations or context to the programmer or anyone else reading the code.

* Comments are extremely helpful when:

  * The code is complex and needs clarification.
  * Other developers are reading or maintaining your code.
  * You revisit your own code after a long time.

Let’s look at an example:

```python
# Declare and initialize variables
x = 10
y = 20

# Print the result of x + y
print(x + y)
```

In this example, the comments clearly explain what each part of the code is doing.
This makes the code easier to understand for others or for your future self.

---

### **2. Single-Line Comments**

A **single-line comment** starts with the `#` symbol and continues to the end of the line.

```python
# This is a single-line comment
x = 10  # This is also a single-line comment
```

#### Key Points:

* A single-line comment can be on its own line or at the end of a line of code.
* It starts with a `#` and does not extend beyond that line.

---

### **3. Multi-Line Comments**

Python does not have a specific syntax for multi-line comments like some other languages, but we can achieve multi-line comments in **two ways**:

#### **Method 1: Using Multiple `#` Symbols**

```python
# Python is a wonderful
# language which is created
# and supported by
# wonderful people across the globe
```

Each line begins with a `#` symbol. This is the most commonly used method.

#### **Method 2: Using Triple Quotes**

We can also use **triple single quotes (`'''`)** or **triple double quotes (`"""`)**:

```python
'''
Python is a wonderful
language which is created
and supported by
wonderful people across the globe
'''
```

* Although triple quotes are meant for multi-line **strings**, Python allows them to be used as comments **if they are not assigned to any variable**.
* These are treated as **docstrings or ignored text** by Python, especially in IDEs like VS Code or PyCharm.

> ⚠️ Note: In the command prompt, Python may print the string enclosed in triple quotes, but in IDEs, this text will not be shown and is treated as a comment.

---

### **4. Uses of Comments**

#### **1. Improve Code Readability**

Comments make your code **easier to read and understand** by explaining what different parts of the code do.

#### **2. Help with Debugging**

During development, you can **temporarily comment out code** that may be causing issues.
Comments can also **explain the logic** behind certain sections, making it easier to spot mistakes.

---

### **Conclusion**

In this presentation, we covered:

* What comments are and why they are important.
* How to write single-line and multi-line comments.
* The practical uses of comments in real-world coding.

Adding meaningful comments is considered a **best practice** in programming.
It helps **you and others** understand the code better and makes maintenance much easier.

---

**Thank you for watching this presentation. See you in the next one!**

---
