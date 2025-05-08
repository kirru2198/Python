# **Statements in Python – Part 1**

Welcome! In this presentation, we will begin our discussion on **statements** in Python. Without any further delay, let’s get started.

---

## **Topics Covered**

1. Introduction to Statements
2. Statement vs Expression

---

## **1. Introduction to Statements**

So, **what is a statement?**

A **statement** is simply an **instruction given to the computer** to perform a specific task. In Python, every line of code that performs an action is considered a statement.

### **Example:**

Let’s open the command prompt and activate the Python interactive shell. Then type:

```python
name = "Sam"
```

Now hit Enter, and type:

```python
print(name)
```

When you press Enter, you’ll see the output:

```
Sam
```

### **Explanation:**

* `name = "Sam"` is a **statement**. It instructs the computer to assign the string `"Sam"` to the variable `name`.
* `print(name)` is also a **statement**. It instructs the computer to display the contents of the variable `name` on the screen.

These are both examples of **statements** because they perform actions.

---

## **2. Statement vs Expression**

Now let’s understand the **difference between a statement and an expression**.

### **Definition:**

* A **statement** is a line of code that performs an **action**.
* An **expression** is a piece of code that is **evaluated for a result**. It **returns a value**.

### **Example:**

```python
x = 10
x = x + 3
```

Let’s break it down:

* `x = 10` is a **statement**. It assigns the value `10` to the variable `x`.
* `x = x + 3` is also a **statement**. It tells the computer to evaluate the expression `x + 3` and assign the result to `x`.

But look closer:

* The part `x + 3` is an **expression** because it is **evaluated** and **produces a value** (in this case, `13`).

So we can say:

* `x = x + 3` is a **statement**.
* `x + 3` inside it is an **expression**.

---

## **Summary:**

* A **statement** is a command that tells the computer to do something.
* An **expression** is a piece of code that produces a value.
* All expressions can be part of a statement, but not all statements are expressions.

---

Thank you for watching this presentation. In the next part, we will explore more about Python statements. See you there!

---
