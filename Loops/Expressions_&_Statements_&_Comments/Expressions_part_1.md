# **Expressions in Python – Part 1**

Welcome! In this presentation, we will dive deep into **expressions in Python**. This is the first part of a series on expressions. Without any further delay, let’s get started.

---

## **Topics Covered**

1. Expressions in Python
2. Constant Expressions
3. Arithmetic Expressions
4. Integral Expressions
5. Floating Point Expressions

---

## **1. Expressions in Python**

### What is an Expression?

An **expression** in Python is a combination of **operands** and **operators** that evaluates to a value. An expression may contain one or more operators and operands.

> **Important:** Every expression **must** evaluate down to a value.

### Example:

Let’s open the Python interactive shell and try the following:

```python
x = 10
x + 3
```

* `x + 3` is an expression.
* It has two operands: `x` and `3`.
* It has one operator: `+`.

Since `x` is assigned to `10`, the expression becomes `10 + 3`, which evaluates to `13`.
Thus, `x + 3` is a valid expression.

---

## **2. Constant Expressions**

### What is a Constant Expression?

A **constant expression** is an expression that contains **only constant values** as operands. The operator(s) can be any operator.

### Example:

```python
10 + 30
```

* Operands: `10` and `30` (both are constants)
* Operator: `+`
* Result: `40`

Since only constants are used, this is a **constant expression**.

---

## **3. Arithmetic Expressions**

### What is an Arithmetic Expression?

An **arithmetic expression** includes:

* Numeric values or strings as operands
* At least one **arithmetic operator** (`+`, `-`, `*`, `/`, `%`, etc.)
* Parentheses (optional), usually for managing order of operations

### Example 1:

```python
x = "neso"
x * 3
```

* `*` is an arithmetic operator (multiplication)
* Operands: a string `"neso"` and an integer `3`
* Result: `'nesonesoneso'`

This is an **arithmetic expression** because it involves an arithmetic operation and evaluates to a value.

### Example 2 (With Parentheses):

Parentheses help in prioritizing operations when multiple operators are present:

```python
(2 + 3) * 4  # Evaluates to 20
```

---

## **4. Integral Expressions**

### What is an Integral Expression?

An **integral expression** always evaluates to an **integer**. Type conversion may be required to ensure the result is an integer.

### Example 1:

```python
x = 5
y = 7.5
result = x + int(y)  # 5 + 7 → 12
```

* `int(y)` converts `7.5` to `7`
* Result: `12` (an integer)
* Hence, this is an **integral expression**

### Example 2:

```python
x = 5
y = '5'
result = x + int(y)  # 5 + 5 → 10
```

* `'5'` (string) is converted to `5` (integer)
* Result: `10`
* This is also an integral expression

---

## **5. Floating Point Expressions**

### What is a Floating Point Expression?

A **floating point expression** evaluates to a **floating point value** (i.e., it contains decimal values). Type conversion may be required.

### Example 1:

```python
x = 10
y = 15.0
result = float(x) + y  # 10.0 + 15.0 → 25.0
```

* Result is a floating point number
* This is a **floating point expression**

> **Note:** Python automatically converts `int` to `float` in mixed operations, but explicit conversion is a good practice.

### Example 2:

```python
x = 10
y = 5
result = x / y  # 10 / 5 → 2.0
```

* `/` always results in a float
* Result: `2.0`
* This is also a **floating point expression**

---

## **Summary**

We have covered the following types of expressions:

* ✅ **Expressions** – combination of operands and operators that evaluate to a value
* ✅ **Constant Expressions** – use only constants as operands
* ✅ **Arithmetic Expressions** – include arithmetic operations
* ✅ **Integral Expressions** – result in an integer value, possibly using type conversion
* ✅ **Floating Point Expressions** – result in a floating point value

---

## **Thank You!**

This concludes Part 1 of the **Expressions in Python** series.
Stay tuned for the next presentation.
Happy Learning! 🚀

---
