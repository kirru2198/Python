## **Python String Methods – Part 6**

Welcome back! Let’s continue our discussion on Python string methods.
This is **Part 6**, and in this session, we’ll explore three important methods:

1. `isalpha()`
2. `isnumeric()`
3. `isalnum()`

At the end, we’ll also look at a **homework problem** for practice.

---

### **1. `isalpha()` Method**

**Purpose:**
The `isalpha()` method returns **`True`** if **all characters** in the string are **alphabetic (A–Z or a–z)**. It returns `False` if any character is not a letter (including digits, spaces, punctuation, etc.).

**Syntax:**

```python
string.isalpha()
```

**Note:** This method **does not take any arguments**.

**Examples:**

```python
"hello2".isalpha()
```

**Output:**

```
False
```

Reason: `2` is not an alphabetic character.

---

```python
"Hello I am Justpreet".isalpha()
```

**Output:**

```
False
```

Reason: It contains **whitespace characters**, which are not alphabetic.

---

```python
"HelloIamJustpreet".isalpha()
```

**Output:**

```
True
```

Reason: All characters are alphabetic, with no digits or spaces.

---

### **2. `isnumeric()` Method**

**Purpose:**
The `isnumeric()` method returns **`True`** if all characters in the string are **numeric (0–9)**. If any character is not a digit, it returns `False`.

**Syntax:**

```python
string.isnumeric()
```

**Examples:**

```python
"2332324".isnumeric()
```

**Output:**

```
True
```

---

```python
"3.14159".isnumeric()
```

**Output:**

```
False
```

Reason: The `.` (decimal point) is not a numeric character.

---

```python
"2/4".isnumeric()
```

**Output:**

```
False
```

Reason: The `/` symbol is not numeric.

---

```python
"-3425".isnumeric()
```

**Output:**

```
False
```

Reason: The `-` (minus sign) is not a numeric character.

---

### **3. `isalnum()` Method**

**Purpose:**
The `isalnum()` method returns **`True`** if all characters in the string are **either alphabetic or numeric** (letters or digits). If the string contains spaces or symbols, it returns `False`.

**Syntax:**

```python
string.isalnum()
```

**Examples:**

```python
"Justpreet20".isalnum()
```

**Output:**

```
True
```

Reason: The string contains both letters and digits, no spaces or symbols.

---

```python
"22324242".isalnum()
```

**Output:**

```
True
```

Reason: All characters are numeric, which is valid.

---

```python
"Justpreet".isalnum()
```

**Output:**

```
True
```

Reason: All characters are alphabetic.

---

```python
"Just Preet".isalnum()
```

**Output:**

```
False
```

Reason: Contains a **space**, which is not allowed.

---

### **📚 Homework Problem**

**Task:**
Determine the output for each line of code given below.
Try solving these **without running them in Python** first. Once you've made your guesses, compare them with actual outputs in the Python interpreter.

```python
print("Python3".isalnum())
print("Python 3".isalnum())
print("123".isnumeric())
print("abc".isalpha())
print("abc123".isalpha())
```

✏️ **Your challenge:**
Write down your answers, then verify them using Python. Post your responses in the comment section if you're in a learning group or community.

---

### **✅ Summary**

| Method        | Description                                      | Returns    |
| ------------- | ------------------------------------------------ | ---------- |
| `isalpha()`   | Checks if all characters are alphabets (A–Z/a–z) | True/False |
| `isnumeric()` | Checks if all characters are digits (0–9)        | True/False |
| `isalnum()`   | Checks if all characters are letters or digits   | True/False |

---

That’s all for this session!
Thank you for watching this presentation, and I’ll see you in the next one.

---
