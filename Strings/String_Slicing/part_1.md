## 🎯 **String Slicing in Python – Part 1**

In this presentation, we will understand **string slicing** in detail. This is **Part One** of the string slicing topic, and we will cover **two key concepts**:

1. What is String Slicing?
2. Slicing with the Third Parameter (Step Value)

---

### 🔹 1. What is String Slicing?

**Definition:**
String slicing is a technique used to extract a **substring** from a string. If you want to access part of a string, Python allows you to do so using **slicing syntax**.

---

### ✏️ **Example 1: Basic Slicing**

Let’s open the **Command Prompt** or any **Python interactive shell** and type:

```python
s = "I am Justpreet"
```

Now, let’s say we want to access the substring `"I am just"`.

```python
s[0:8]
```

**Explanation:**

* `0` is the **start index**.
* `8` is the **end index + 1** (i.e., 7 + 1), since slicing in Python **excludes** the end index.
* Hence, `s[0:8]` gives us `"I am just"`.

**Important Rule:**
In slicing syntax `s[start:end]`, the `end` index is **not inclusive**. That’s why we write `8` to get characters up to index `7`.

---

### 🔹 2. Slicing with the Third Parameter (Step Value)

Python also allows a **third parameter** in slicing: the **step value**.

```python
s[start:end:step]
```

* `start`: Index to begin slicing from.
* `end`: Index to stop slicing (exclusive).
* `step`: Number of characters to skip (default is `1`).

---

### ✏️ **Example 2: Slicing with Step Value**

```python
s = "I am Justpreet"
s[0:8:2]
```

**What does this do?**

* `0`: Start at index 0.
* `8`: Go up to index 7.
* `2`: Take every second character.

**Output:**

```
'Ia a'
```

**How?**

* Start at index 0 → `'I'`
* Skip index 1 → `' '`, take index 2 → `'a'`
* Skip index 3 → `'m'`, take index 4 → `' '`
* Skip index 5 → `'J'`, take index 6 → `'u'`
* Stop before index 8.

---

### 🎯 Understanding Step Value

If step value = `n`, Python **includes every nth character**, starting from the `start` index, and skipping `n - 1` characters in between.

---

### 🔄 Homework Problem

Try this:

```python
s = "I am Justpreet"
s[2:10:2]
```

👉 What will be the output?
Analyze it character by character.

---

## 🧪 Advanced Examples

---

### ✅ Example 3: Repeating a String

```python
s = "abc" * 3
print(s)
# Output: 'abcabcabc'
```

---

### ✅ Example 4: Omitting Start and End

```python
s[::3]
```

* Start and end are omitted → slice the **entire string**.
* Step = 3 → take every 3rd character.

**Output:**
It gives every third character from the string: `'aaa'`

---

### ✅ Example 5: Only Start Provided

```python
s[1::3]
```

* Start from index 1.
* Step = 3 → every third character.

**Output:**
Gives you `'bbb'`

---

### ✅ Example 6: Only End Provided

```python
s[:5:3]
```

* Start from beginning (default is 0).
* Go up to index 4.
* Step = 3 → every third character.

**Output:**
Gives you `'aa'`

---

## ✅ Summary

In this part, we covered:

* What string slicing is
* How to use `start`, `end`, and `step` values
* The effect of providing or omitting parameters
* Several practical examples

👉 **Practice Tip:** Try changing the start, end, and step values with different strings to see how the slicing behaves.

---

**Thanks for watching this presentation.**
See you in the next one where we’ll explore more advanced slicing techniques!

---
