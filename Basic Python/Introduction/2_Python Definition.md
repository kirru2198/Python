# 📘 Python Programming – Lecture 2: Python Definition

Welcome back! In the previous lecture, we introduced Python Programming. In this session, we’ll cover an important foundational topic:

---

## 🧠 **Topic of This Lecture**
- **Definition of Python**

We’ll break down this definition word by word so you understand exactly what Python is, how it works, and why it's so popular.

---

## 📖 **Definition of Python**

> **Python is an interpreted, general-purpose (or multi-purpose), high-level programming language with easy syntax and dynamic semantics.**

Let’s understand the meaning of this definition, step by step.

---

## 👨‍🏫 Creator of Python

- **Python was created by Guido van Rossum** between **1985 and 1990**.
- The name **Python** was inspired not by the snake 🐍, but by **“Monty Python’s Flying Circus,”** a British comedy show that Guido enjoyed.

---

## 🔍 Understanding the Definition

There are two types of programming languages -- Interpreted and Compiled programming language

- Interpreted rogramming language is a language which uses Interpretr for its translation
-  Compiled programming language is a language which uses compiler for its translation
-  compiler and Interpretr are translators --- they are use to translate the code written in one programming language to the code written in another programming language

### 🗣️ **1. Interpreted Language**

- Python is an **interpreted language**, not a compiled one.
- It uses an **interpreter** to translate code into machine-readable instructions.

#### ✅ Why is Translation Needed?
- Humans write code in a language we understand (like Python, Java, etc.).
- **Computers understand only machine code (0s and 1s)**.
- **Interpreter**: Translates human code → machine code line by line.
- **Compiler**: Translates entire code → machine code at once.

> we need to translate the code which we can understand to the code which machines can understand
> - so you can think of a translator as a device or a machine which takes source code or the code which we humans can understand as input and in response it generates machine code as output
> - machine code is the code which machines or computers can understand
> - so this is the reason why translation is needed

<img width="377" alt="image" src="https://github.com/user-attachments/assets/b62f2fa1-39df-4194-b04d-8e971f4f9771" />


Python uses an **interpreter** — so it translates code line-by-line when the program is run.

---

### 🌐 **2. General-Purpose / Multi-Purpose Language**

- Python is **not limited** to a single domain.
- You can use Python for:
  - 🌐 Web Development
  - 🤖 Robotics
  - 🧠 Artificial Intelligence
  - 📱 Mobile App Development
  - 💻 Desktop Applications
  - 🧪 Data Science and more!

Hence, Python is called **general-purpose** because it can be used anywhere.

---

### 🔝 **3. High-Level Language**

> Python is a High-Level programming Language which means that we humans can understand this language without any problem

>On the other hand a low-level programming Language is a Language which only machines can understand well (by the way machines can understrand the lnaguage of 0's and 1's and we humans are not capable of understanding that language) 

- Python is **easy for humans to read and write**.
- Contrast:
  - High-Level Code (like Python): `area = length * breadth`
  - Low-Level Code (machine language): `01010100 10100011 ...`

Example:
```python
length = 50
breadth = 20
area = length * breadth
print(area)
```

<img width="384" alt="image" src="https://github.com/user-attachments/assets/11496629-29ce-4b6f-a3ee-b7fb72f458af" />


This is easy for **humans** to understand. That’s what makes Python a **high-level language**.

---

### 🧾 **4. Easy Syntax**

Python code is:
- Clean
- Concise
- Free from complex syntax

#### Example Comparison:

**C Code:**
```c
int x = 10;
int y = 5;
printf("%d", x + y);
```
> "%d" is the placeholder for the value which we want to print -- in this case we want to print 15 on the screen that is why this "%d" is the placeholder for the value 15. Here, d stands for decimal. 

**Python Code:**
```python
x = 10
y = 5
print(x + y)
```

**Python Advantages:**
- No need to declare variable types
- No semicolons
- No formatting placeholders like `%d`
- Uses plain `print()` for output

---

### 🔄 **5. Dynamic Semantics**

dynamic Semantics mean that variables are Dynamic objects in Python. 

Python is **dynamically typed**:
- You **don’t need to declare types** when creating variables.
- Variables can **change type** during program execution.

#### Example:

```python
x = 10       # x is an integer
x = 10.78    # now x is a float
x = "hello"  # now x is a string
```

Python allows this flexibility because it **assigns data types at runtime**, not at compile time.

### 🆚 Static Typing in C:

**C Code:**
```c
int x = 10;
x = 10.78;  // Only 10 gets stored; the decimal part is lost
```

In C (a statically typed language), you **must declare the type** of variables and it can’t change dynamically.

---

## ✅ Summary of Python Definition

> Python is:
- ✅ **Interpreted**: Uses an interpreter to run code line-by-line.
- ✅ **General-Purpose**: Can be used across domains like web, AI, robotics, etc.
- ✅ **High-Level**: Easy for humans to read and write.
- ✅ **Easy Syntax**: Less complex syntax than other languages like C/C++.
- ✅ **Dynamic Semantics**: No need for type declarations; types can change.

---

## 🎉 Conclusion

Congratulations! You’ve now understood what Python **is** and what makes it **powerful and easy to learn**.

Next, we’ll move deeper into the world of Python and start learning its **core concepts**.

📌 **Stay tuned for the next lecture.**  
Thank you for watching!

---
