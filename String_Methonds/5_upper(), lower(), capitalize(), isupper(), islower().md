Sure! Here's a well-structured and clearly written version of your presentation content on string methods in Python:

---

## **Understanding More String Methods in Python**

In this presentation, we will learn five important string methods in Python:

1. `upper()`
2. `lower()`
3. `capitalize()`
4. `isupper()`
5. `islower()`

Let’s go through each method one by one with detailed explanation and examples.

---

### **1. `upper()` Method**

**Purpose:**
The `upper()` method is used to convert **all the letters** of a string to **uppercase**.

**Syntax:**

```python
string.upper()
```

**Note:** This method **does not take any arguments**.

**Example:**

```python
s = "hello I am Justpreet"
print(s.upper())
```

**Output:**

```
HELLO I AM JUSTPREET
```

---

### **2. `lower()` Method**

**Purpose:**
The `lower()` method converts **all the letters** in a string to **lowercase**.

**Syntax:**

```python
string.lower()
```

**Example:**

```python
s = "HELLO I AM JUSTPREET"
print(s.lower())
```

**Output:**

```
hello i am justpreet
```

---

### **3. `capitalize()` Method**

**Purpose:**
The `capitalize()` method returns a string where the **first character** is **uppercase** and the **rest of the characters are lowercase**.

**Syntax:**

```python
string.capitalize()
```

**Examples:**

```python
s = "maruti SUZUKI"
print(s.capitalize())
```

**Output:**

```
Maruti suzuki
```

If the string starts with a number, `capitalize()` does nothing to it:

```python
s = "29marutisuzuki"
print(s.capitalize())
```

**Output:**

```
29marutisuzuki
```

---

### **4. `isupper()` Method**

**Purpose:**
The `isupper()` method checks if **all characters** in the string are **uppercase**.
It returns a **Boolean value**: `True` if all characters are uppercase, `False` otherwise.

**Syntax:**

```python
string.isupper()
```

**Examples:**

```python
s = "HELLO"
print(s.isupper())
```

**Output:**

```
True
```

```python
s = "Hello Friends"
print(s.isupper())
```

**Output:**

```
False
```

---

### **5. `islower()` Method**

**Purpose:**
The `islower()` method checks if **all characters** in the string are **lowercase**.
It returns a **Boolean value**: `True` if all characters are lowercase, `False` otherwise.

**Syntax:**

```python
string.islower()
```

**Examples:**

```python
s = "hello"
print(s.islower())
```

**Output:**

```
True
```

```python
s = "Hello Friends"
print(s.islower())
```

**Output:**

```
False
```

---

### **Summary**

| Method         | Purpose                                | Returns    |
| -------------- | -------------------------------------- | ---------- |
| `upper()`      | Converts all characters to uppercase   | New string |
| `lower()`      | Converts all characters to lowercase   | New string |
| `capitalize()` | First letter uppercase, rest lowercase | New string |
| `isupper()`    | Checks if all characters are uppercase | True/False |
| `islower()`    | Checks if all characters are lowercase | True/False |

---

Thank you for watching this presentation. In the next session, we will explore more Python string methods. See you next time!

---
