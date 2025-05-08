# **Statements in Python – Part 2**

Welcome back! In this presentation, we will **continue our discussion on statements in Python**. This is Part 2 of the topic.

---

## **Topics Covered**

1. Multi-line Statements
2. Homework Problem

---

## **1. Multi-line Statements**

### **What are Multi-line Statements?**

In Python, **multi-line statements** are statements that are **spread across multiple lines**. This is helpful when writing long lines of code for better readability.

Python allows multi-line statements in several ways:

* Using a **continuation character (`\`)**
* Using **parentheses `()`**
* Using **square brackets `[]`**
* Using **curly brackets `{}`**

Let’s go through each method one by one.

---

### **Method 1: Using the Continuation Character (`\`)**

Let's open the **Python interactive shell** and type:

```python
x = 10 + 20 + 30 + \
    40 + 50 + 60 + 70 + \
    80 + 90 + 100
```

* The **backslash (`\`)** tells Python that the statement continues on the next line.
* After entering each line with `\`, Python shows `...` to indicate that it expects more input.

Now, type:

```python
print(x)
```

**Output:**

```
550
```

This shows that the sum of all numbers was successfully calculated using a multi-line statement.

---

### **Method 2: Using Parentheses `()`**

You can also use **parentheses**, which automatically allow multi-line statements without the need for a backslash.

```python
x = (
    10 + 20 + 30 +
    40 + 50 + 60 +
    70 + 80 + 90 + 100
)
```

Now, print the result:

```python
print(x)
```

**Output:**

```
550
```

Python understands that the statement continues until the closing parenthesis.

---

### **Method 3: Using Square Brackets `[]`**

Square brackets are typically used for **lists**, and they naturally support multi-line declarations.

```python
x = [
    "Sam", 
    "Pam",
    "Brad", 
    "Harry"
]
```

Now print:

```python
print(x)
```

**Output:**

```
['Sam', 'Pam', 'Brad', 'Harry']
```

This list contains four elements, written across multiple lines.

---

### **Method 4: Using Curly Brackets `{}`**

Curly brackets are used to create **sets** or **dictionaries**, and like lists, they support multi-line formatting.

```python
x = {
    10 + 20 + 30 +
    40 + 50 + 60 +
    70 + 80 + 90 + 100
}
```

Now print:

```python
print(x)
```

**Output:**

```
{550}
```

Here, we’ve created a **set** with a single value `550`.

---

## **2. Homework Problem**

Let’s test your understanding.

### **Task:**

Identify which of the following lines are **statements** and which are **expressions**:

```python
x = 5
y = x + 2
x + 2
print(y)
```

* Go through each line and determine:

  * Which ones are **statements** (perform an action)?
  * Which ones are **expressions** (evaluate to a value)?

📝 **Post your answers in the comment section!**

---

## **Summary**

* We explored how to write **multi-line statements** using:

  * Continuation character (`\`)
  * Parentheses `()`
  * Square brackets `[]`
  * Curly brackets `{}`
* You now understand how Python handles multi-line code.
* Don’t forget to complete the **homework problem**!

---

Thank you for watching this presentation. I’ll see you in the next one!

---
