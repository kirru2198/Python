## 📘 Understanding `break` and `continue` Statements in Python

Hello everyone!
In this presentation, we will learn how the `break` and `continue` statements work in Python.

So, without any further delay, let's get started!

---

### ✅ Topics Covered:

1. **The `break` Statement**
2. **The `continue` Statement**

---

## 🔹 The `break` Statement

Let’s begin with the `break` statement.

The `break` statement is used to **terminate a running loop** prematurely. When a specific condition is met, the `break` statement can be used to exit the loop immediately.

---

### 🔸 Example 1: Print Numbers from 0 to 50

Let’s say we want to print numbers from 0 to 50, but we first generate a list of numbers from 0 to 99.

There are two ways to generate this list:

* Manually type the numbers.
* Use the `range()` function with `list()`.

```python
numbers = list(range(0, 100))
```

Now we only want to print numbers **from 0 up to 50**:

```python
for number in numbers:
    if number > 50:
        break
    print(number, end=' ')
```

### Output:

```
0 1 2 3 4 5 6 7 8 9 10 ... 50
```

Explanation:

* As soon as the number becomes greater than 50, the `break` statement is executed.
* This stops the loop immediately, and no further numbers are printed.

---

### 🔸 Example 2: Infinite Loop with User Input

Now let’s consider an **infinite loop** that stops only when the user enters `"Q"`.

```python
while True:
    num = input("Enter a number (Q to quit): ")
    if num == "Q":
        break
    print(num)
```

### Output Behavior:

* User enters `10` → Output: `10`
* User enters `20` → Output: `20`
* User enters `Q`  → Loop terminates.

This is useful when we don’t know the loop termination condition in advance and want it to depend on user input.

---

## 🔹 The `continue` Statement

The `continue` statement is used to **skip the current iteration** of a loop and move to the next one.

---

### 🔸 Example 1: Print 0, 1, and 3 (Skip 2 and 4)

We want to print numbers from 0 to 4 but skip 2 and 4:

```python
for i in range(5):
    if i == 2 or i == 4:
        continue
    print(i)
```

### Output:

```
0
1
3
```

Explanation:

* When `i` is 2 or 4, the `continue` statement is executed, skipping the `print()`.

---

### 🔸 Example 2: Print Even Numbers Only (Using `while` Loop)

Now let’s print even numbers from 1 to 10 using a `while` loop:

```python
n = 0

while n <= 10:
    n += 1
    if n % 2 != 0:
        continue
    print(n, end=' ')
```

### Output:

```
2 4 6 8 10
```

Explanation:

* If the number is odd (`n % 2 != 0`), the loop skips that iteration.
* Only even numbers are printed.

---

## ✅ Summary

* Use `**break**` to exit a loop prematurely.
* Use `**continue**` to skip the current iteration and proceed with the next.

These control flow statements are powerful tools for managing loop behavior in real-world programs.

---

Thank you for watching this presentation!
See you in the next one.

---
