## 🎓 **Explicit Type Conversion in Python**

Welcome to this presentation on **explicit type conversion** in Python. In the previous session, we explored **implicit type conversion**, where Python automatically converts one data type to another without any intervention from the programmer. In this session, we’ll delve into **explicit type conversion**, where the **programmer manually performs the conversion**.

Let’s begin by quickly revisiting the **homework problem** from our previous lecture.

---

### 🧠 **Homework Problem Recap**

Here’s the code snippet we were supposed to analyze:

```python
x = 10
y = 20
total = x + y
print("The total is: " + total)
```

#### ❌ Output:

This code throws an error:

```
TypeError: can only concatenate str (not "int") to str
```

#### ✅ Why the Error Occurs:

* The first three lines are valid. `x` and `y` are assigned integer values, and `total` correctly stores their sum.
* The issue arises in the `print` statement:

  * `"The total is: "` is a string.
  * `total` is an integer.
  * The `+` operator, when used between a string and an integer, tries to concatenate them—but Python does **not** allow **implicit conversion** from `int` to `str`.

> **Note:** Python avoids implicitly converting `int` to `str` to prevent unintended behavior and potential program crashes. Instead, it raises an error to alert the programmer.

---

### 🔄 **Why Implicit Conversion Didn’t Work Here**

In implicit conversion:

* Python automatically converts from a **lower** data type to a **higher** one (like `int` to `float`) to avoid data loss.
* But converting from `int` to `str` can change the program’s meaning and logic, so Python does **not** perform this implicitly.

Thus, to make this code work, the programmer must **explicitly** convert the `int` to a `str`.

---

## 🛠️ **Explicit Type Conversion Using `int()`**

Now let’s understand **explicit type conversion**, also known as **type casting**.

> **Definition:**
> Explicit type conversion refers to the process where the **programmer manually converts** one data type into another using Python's built-in functions.

For example, to convert a value to an integer, we use the `int()` function.

---

### 🧪 **Basic Syntax of `int()`**

```python
int(value, base)
```

* **`value`**: The value to convert.
* **`base`** *(optional)*: The number system base (e.g., 2 for binary, 8 for octal).

---

### ✅ **Example 1: Convert String to Integer**

```python
x = '110'
print(type(x))  # Output: <class 'str'>

x = int(x)
print(x)        # Output: 110
print(type(x))  # Output: <class 'int'>
```

---

### ✅ **Example 2: Use `base` Argument in `int()`**

```python
x = '110'
x = int(x, 2)  # Treat '110' as binary
print(x)       # Output: 6 (binary 110 = decimal 6)
print(type(x)) # Output: <class 'int'>
```

* Here, we **explicitly** tell Python to treat the input as **binary** by passing `2` as the base.
* Python then converts the binary number `'110'` to its decimal equivalent, which is `6`.

---

## 📌 Summary

* **Implicit type conversion** is automatic and only occurs when **no precision is lost** and the conversion is safe.
* **Explicit type conversion** is performed **manually** using functions like `int()`, `float()`, `str()`, etc.
* Python avoids implicit conversions that could result in **unexpected behavior** or **data loss**—for example, converting `int` to `str`.

---

## 🏁 Conclusion

In this presentation, we:

* Reviewed the homework problem and understood the cause of the `TypeError`.
* Learned how **explicit type conversion** works, especially using the `int()` function.
* Explored examples of converting both string values and binary values to integers using `int()`.

---
