## 📘 String Methods in Python: `split()` and `rsplit()`

Welcome back! In our previous session, we discussed `lstrip()` and `rstrip()` methods in Python. In this presentation, we will continue exploring more string methods. Today’s focus will be on:

1. `split()` method
2. `rsplit()` method

After covering both, we’ll conclude with a homework problem to test your understanding.

---

### 🔹 1. `split()` Method

The `split()` method is used to divide a string into a list of substrings.

#### **Definition:**

```python
string.split(separator, maxsplit)
```

* `separator`: (optional) The delimiter at which the string will be split. By default, it's any whitespace character.
* `maxsplit`: (optional) The maximum number of splits to perform. Default is `-1`, meaning "no limit".

#### **Example:**

```python
text = "Hello!$I$am$Just Breathe"
result = text.split("$", 2)
```

**Explanation:**

* The separator is `$`
* The maximum number of splits is 2

So, the split will happen only at the first two `$` symbols:

**Result:**

```python
['Hello!', 'I', 'am$Just Breathe']
```

Here’s how it works:

1. `'Hello!'` → First item (before first `$`)
2. `'I'` → Second item (between first and second `$`)
3. `'am$Just Breathe'` → Third item (everything after the second `$`)

If `maxsplit` were `3`, it would split again at the next `$`.

#### **Another Example (No Arguments):**

```python
text = "Hello! I am Just Breathe"
result = text.split()
```

**Default behavior:**

* Separator: any whitespace
* Maxsplit: unlimited

**Result:**

```python
['Hello!', 'I', 'am', 'Just', 'Breathe']
```

---

### 🔹 2. `rsplit()` Method

The `rsplit()` method is similar to `split()`, but it splits the string starting **from the right**.

#### **Definition:**

```python
string.rsplit(separator, maxsplit)
```

* It accepts the same two arguments: `separator` and `maxsplit`

#### **Example:**

```python
text = "Hello!$I$am$Just Breathe"
result = text.rsplit("$", 2)
```

**Explanation:**

* Separator is `$`
* Max split = 2
* But this time, the splitting starts from the **right**.

**Result:**

```python
['Hello!$I', 'am', 'Just Breathe']
```

Here’s what happens:

1. `'Just Breathe'` → Last item (after last `$`)
2. `'am'` → Second last item
3. `'Hello!$I'` → First item (everything before the second-last `$`)

**Key Difference:**

* `split()` starts splitting from the **left**
* `rsplit()` starts splitting from the **right**

---

### 📚 Homework Problem

**Question:**
What is the output of the following code?

```python
text = "Hello! I am Just Breathe"
print(text.rsplit())
```

**Hint:**
No arguments are passed to `rsplit()`, so it behaves like `split()` using default whitespace separation and unlimited splits.

---

### ✅ Summary

* `split()` divides a string starting from the **left**
* `rsplit()` divides a string starting from the **right**
* Both methods accept two optional arguments: `separator` and `maxsplit`

---

Thank you for watching this presentation. I hope the concepts of `split()` and `rsplit()` are now clear. See you in the next session!

---
