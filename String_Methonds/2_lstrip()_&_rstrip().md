### String Methods in Python – Part 2

In the previous session, we discussed the `strip()` method. We learned that:

* The `strip()` method removes **leading and trailing white spaces** by default.
* If we provide specific characters as an argument, `strip()` will remove those **characters from the beginning and end of the string only**—not from the middle.

Now, let’s move forward and explore **two more string methods**:

* `lstrip()`
* `rstrip()`

We'll also solve some problems and conclude with a homework exercise.

---

### 1. What is `lstrip()`?

The `lstrip()` method removes **leading white spaces** from a string (i.e., spaces from the left side).

* The **"L"** in `lstrip` stands for **"Left"**.
* By default, it removes white spaces from the beginning of the string.
* We can also pass specific characters as an argument to remove those from the **start of the string only**.

**Example:**

```python
>>> "   Hello World   ".lstrip()
'Hello World   '
```

Only the leading spaces are removed; trailing spaces remain.

If we provide characters, `lstrip()` removes **all matching characters from the start**, **in any order**, **until it hits a character not in the list**.

---

### 2. What is `rstrip()`?

The `rstrip()` method removes **trailing white spaces** (i.e., spaces from the right side).

* The **"R"** in `rstrip` stands for **"Right"**.
* By default, it removes only trailing white spaces.
* We can also pass specific characters to remove them from the **end of the string only**.

**Example:**

```python
>>> "   Hello World   ".rstrip()
'   Hello World'
```

Only the trailing spaces are removed; leading spaces remain.

---

### 3. Practice Problems

#### **Problem 1:**

```python
>>> "  Solving any problem is an art.  ".strip(". ")
```

**Explanation:**
We’re passing a string containing `"."` and a space as the argument.
So, it will remove all leading/trailing white spaces and dots.

**Output:**

```
'Solving any problem is an art'
```

---

#### **Problem 2:**

```python
>>> "  Solving any problem is an art.  ".strip("")
```

**Explanation:**
We're passing an **empty string** as the argument. This means **no characters** will be stripped.

**Output:**

```
'  Solving any problem is an art.  '
```

---

#### **Problem 3: Fill in the Blanks**

```python
str = "  I am Just Breathe  ."

str.lstrip(" Iam.")        # Output?
str.rstrip(" Iam.")        # Output?
str                        # Output?
```

**Step-by-step Explanation:**

1. **Original string:**

```
"  I am Just Breathe  ."
```

2. **`str.lstrip(" Iam.")`:**

   * Removes characters `" "`, `"I"`, `"a"`, `"m"`, `"."` **from the start**.
   * Stops when it hits `"J"` (not in the given set).
   * **Result:** `'Just Breathe  .'`

3. **`str.rstrip(" Iam.")`:**

   * Removes `" "`, `"I"`, `"a"`, `"m"`, `"."` **from the end**.
   * Stops when it hits `"e"` (not in the set).
   * **Result:** `'  I am Just Breathe'`

4. **`str`:**

   * Still holds the original value since `.lstrip()` and `.rstrip()` don’t modify it in place.
   * **Result:** `'  I am Just Breathe  .'`

---

### 4. Homework Problem

```python
>>> "My name is JustPreet".rstrip("my ")
```

**Task:**
Determine the output of the above code.

**Hint:**

* `rstrip("my ")` will remove **any combination** of the characters `"m"`, `"y"`, and `" "` **from the end only**.
* Remember: Python string methods are **case-sensitive**.

Try solving it yourself before moving to the next session!

---

### Summary

In this session, we:

* Explored `lstrip()` and `rstrip()` methods.
* Understood how they differ from `strip()`.
* Practiced with real-world examples and edge cases.
* Tackled tricky string manipulation problems.

Thank you for watching this presentation. See you in the next one!
