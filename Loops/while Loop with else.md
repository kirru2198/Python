### 🎯 Title: Understanding `while` Loop with `else` in Python

Hello everyone!

In this presentation, we will explore an important concept in Python: the **`while` loop with `else`** clause.
So, without any further delay, let's dive right in.

---

## 🔹 Topics Covered:

1. Introduction to `while` loop with `else`
2. Use of `while` loop with `else` through a practical example

---

## 1️⃣ Introduction to `while` loop with `else`

As we already know, the `while` loop in Python allows us to execute a block of code repeatedly **as long as a condition is true**. Once the condition becomes false, the loop terminates.

### ✅ Normal Termination vs Break (Abnormal Termination)

There are **two ways** a `while` loop can terminate:

* **Normal Termination**: When the `while` condition becomes false.
* **Abnormal Termination**: When a `break` statement is encountered inside the loop.

Now, suppose we want to execute a specific block of code **only when the loop completes normally** — that is, without encountering a `break` statement. In such cases, Python provides the `else` clause with the `while` loop.

### 🧠 Important Concept:

> The `else` block in a `while` loop executes **only when the loop ends normally** (i.e., the condition becomes false), and **not when the loop is terminated using `break`**.

Let’s see the **syntax** of `while` with `else`:

```python
while condition:
    # loop body
    if some_condition:
        break  # abnormal termination
else:
    # this block runs only if loop was not broken
```

---

## 2️⃣ Use of `while` loop with `else` – Practical Example

Let’s look at an example to understand its usage better.

### 📝 Problem Statement:

We have a list of fruits:

```python
fruits = ["apple", "banana", "mango", "strawberry"]
```

We need to **check whether "orange" is present** in the list or not.
If it is present, print: `"Orange is available"`
If not, print: `"Orange is not available"`

Let’s write the Python code for this:

### ✅ Version 1 – Using `while` with `break` and `else`

```python
fruits = ["apple", "banana", "mango", "strawberry"]
index = 0

while index < len(fruits):
    if fruits[index] == "orange":
        print("Orange is available")
        break  # terminate loop if found
    index += 1
else:
    # This will run only if the loop wasn't broken
    print("Orange is not available")
```

### 💡 Explanation:

1. We start with `index = 0` and loop while `index < len(fruits)`.
2. In each iteration, we compare `fruits[index]` with `"orange"`.
3. If a match is found, we print `"Orange is available"` and exit the loop using `break`.
4. If no match is found and the loop completes, the `else` block is executed, printing `"Orange is not available"`.

---

### ⚠️ Why Not Just Use a Print After the Loop?

If we placed `print("Orange is not available")` **outside** the loop without using `else`, then even in the case where orange *was* found (and we used `break`), that message would still be printed. That would be incorrect behavior.

Using `else` helps us avoid that by executing the "not found" message **only when the loop wasn’t interrupted** by a `break`.

---

## ✅ Summary

* The `else` clause with a `while` loop runs **only** when the loop ends naturally.
* It is **skipped** if the loop is terminated by a `break`.
* This is especially useful when searching for something in a loop and performing different actions based on whether it was found.

---

### 🙌 Final Thoughts

I hope this explanation of the `while` loop with `else` was helpful. It’s a simple yet powerful concept that makes your code cleaner and more readable.

Thank you for watching this presentation!
See you in the next one. 👋

---
