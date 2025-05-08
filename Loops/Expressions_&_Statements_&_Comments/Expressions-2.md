# **Expressions in Python – Part 2**

Welcome back! In the previous part, we explored what expressions are in Python and looked at some of their types such as:

* Integral expressions
* Constant expressions
* Arithmetic expressions
* Floating-point expressions

In this presentation, we will continue our discussion and explore more types of expressions in Python.

---

## **Topics Covered**

1. Relational Expressions
2. Logical Expressions
3. Bitwise Expressions
4. Combinational Expressions
5. Precedence of Operators

Let’s dive into each of these topics.

---

## **1. Relational Expressions**

### **What are Relational Expressions?**

* Relational expressions are also known as **Boolean expressions** because they always return a **Boolean value** (`True` or `False`).
* These expressions involve **relational operators**.
* Instead of just simple values like `10`, `20`, etc., **arithmetic expressions** or other expressions can also be used as operands.

### **Example:**

```python
10 + 13 <= 2 + 3
```

* `10 + 13` evaluates to `23`
* `2 + 3` evaluates to `5`
* The expression becomes: `23 <= 5` → which is `False`

Hence, the result of this relational expression is `False`.

---

## **2. Logical Expressions**

### **What are Logical Expressions?**

* Logical expressions consist of **relational expressions connected by logical operators**.
* These operators include: `and`, `or`, and `not`.
* Just like relational expressions, logical expressions **always return a Boolean value**.

### **Example:**

```python
10 < 13 and 1 == 1
```

* `10 < 13` → `True`
* `1 == 1` → `True`
* Since both are `True` and the logical operator is `and`, the final result is `True`.

---

## **3. Bitwise Expressions**

### **What are Bitwise Expressions?**

* Bitwise expressions involve **bitwise operators** like `&`, `|`, `^`, `~`, `<<`, `>>`.
* These operate at the **bit level** and are used mainly with integers.

### **Example:**

```python
10 << 2
```

* The left shift operator `<<` shifts bits to the left.
* This is equivalent to multiplying `10` by `2^2`:

  * `10 * 4 = 40`
* So the result is `40`.

---

## **4. Combinational Expressions**

### **What are Combinational Expressions?**

* A combinational expression is a **mix of different types of expressions** (arithmetic, bitwise, logical, etc.) in one line.
* These require an understanding of **operator precedence** to evaluate correctly.

### **Example:**

```python
x = 10
y = 20
z = y + (x << 1) - x * 3
```

Let’s break it down:

1. `x << 1` → `10 << 1` = `10 * 2 = 20`
2. `x * 3` → `10 * 3 = 30`
3. So the expression becomes: `20 + 20 - 30`
4. Evaluate left to right: `40 - 30 = 10`

So, `z` gets the value `10`.

---

## **5. Precedence of Operators**

Understanding operator precedence is **crucial** when working with complex expressions.

### **Operator Precedence (Highest to Lowest):**

1. **Parentheses**: `()`
2. **Exponentiation**: `**`
3. **Unary Operators**: `+x`, `-x`, `~x`
4. **Multiplication, Division, Floor Division, Modulus**: `*`, `/`, `//`, `%`
5. **Addition and Subtraction**: `+`, `-`
6. **Bitwise Shifts**: `<<`, `>>`
7. **Bitwise AND**: `&`
8. **Bitwise XOR**: `^`
9. **Bitwise OR**: `|`
10. **Comparison Operators**: `<`, `<=`, `>`, `>=`
11. **Equality Operators**: `==`, `!=`
12. **Identity and Membership Operators**: `is`, `is not`, `in`, `not in`
13. **Logical NOT**: `not`
14. **Logical AND**: `and`
15. **Logical OR**: `or`
16. **Assignment Operators**: `=`, `+=`, `-=`, etc. (Lowest precedence)

---

## **Conclusion**

In this part, we have covered:

* **Relational Expressions**
* **Logical Expressions**
* **Bitwise Expressions**
* **Combinational Expressions**
* **Operator Precedence**

These topics form a strong foundation for understanding how complex expressions are evaluated in Python. Make sure to practice these concepts to reinforce your learning.

Thank you for watching this presentation. See you in the next one!

---
