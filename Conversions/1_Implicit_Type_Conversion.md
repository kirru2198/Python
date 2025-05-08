# 📘 Implicit Type Conversion in Python

Hello friends,
Welcome to this presentation! In this session, we will understand what **implicit type conversion** is in Python. After that, we will look at the **homework problem** for this lecture.

---

## 📌 What is Implicit Type Conversion?

**Implicit type conversion** refers to Python’s ability to automatically convert one data type to another without any explicit direction from the programmer. This process is entirely automatic and happens **behind the scenes** when Python detects that conversion is necessary for a particular operation.

### ✅ Key Characteristics:

* **Automatic**: No manual code or conversion functions are needed.
* **Triggered by necessity**: Conversion happens only when needed to avoid type mismatches.
* **Follows a strict rule**: Python always converts the **lower data type** to the **higher data type** to prevent data loss.

---

## 🔄 Rule of Conversion

Python follows a simple principle during implicit conversions:

> 🔁 **Lower data types** (e.g., `int`) are automatically promoted to **higher data types** (e.g., `float`) if required.

Let’s see an example.

---

## 🧪 Example 1: Mixing `int` and `float`

```python
5 + 10.98
```

* `5` is an `int`
* `10.98` is a `float`

Python **implicitly converts** `5` to `5.0` and then performs the addition:

```python
Result: 15.98
```

This happens because:

* `float` is a higher data type than `int`
* Python avoids converting `float` to `int` since it would result in **loss of precision**

---

## 🧠 Hypothetical Scenario: Reverse Rule (Not in Python)

Let’s imagine Python followed the opposite rule: converting **higher data types to lower**.

In that case:

```python
5 + 10.98  # Hypothetical result: 15 (since 10.98 → 10)
```

But Python **does not do this** because:

* Converting `10.98` to `10` loses data (`0.98`)
* It violates Python's design principle to avoid data loss

So always remember:

> **Python does not implicitly convert `float` to `int`**

---

## 🔁 Division in Python

Another case of implicit type conversion involves the **division operator (`/`)**.

```python
10 / 5
```

Both operands are `int`, but the result is:

```python
2.0 (float)
```

Why?

* Because **division always results in a `float`**, regardless of operand types
* The result type is influenced not just by operand types, but by the **operator**

### 💡 Note:

If you want integer division, use the **floor division operator `//`**.

```python
10 // 5  # Result: 2 (int)
```

---

## ⚙️ Implicit Conversion in C vs Python

In **C programming**, implicit conversion from a higher to a lower data type **is allowed**, even though it may lead to **data loss**.

Example in C:

```c
int x;
x = 98.5;  // float to int conversion
```

* This is allowed in C.
* `x` stores `98` (fractional part `.5` is lost)
* The **responsibility of data loss** lies with the **programmer**, not the compiler

### 🚫 In Python:

* We don’t explicitly declare data types
* Python **never implicitly converts `float` to `int`**
* This prevents **accidental precision loss**

---

## 📝 Summary

* Python performs **implicit type conversion** when needed.
* It always converts from **lower to higher** data types (`int` → `float`, not vice versa).
* Division (`/`) always results in a `float`, regardless of operand types.
* Python avoids data loss by **not converting `float` to `int` implicitly**, unlike C.

---

## 🧠 Homework Problem

Determine the output of the following lines of code. Try to work them out manually before testing them in your Python shell.

```python
print(5 + 10.2)
print(8 / 4)
print(3 // 2)
print(4 + True)
```
