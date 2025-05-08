# Python String Methods – Part 1: `strip()` Method

In this session, we will begin our exploration of string methods in Python. This is **Part 1**, and we will focus on one important method: the **`strip()`** method.

---

## What is the `strip()` Method?

The `strip()` method is a built-in **string method** in Python. It is used to **remove leading and trailing characters** from a string. By default, it removes **leading and trailing white spaces**.

---

## Basic Usage of `strip()`

Let’s understand this with a simple example.

1. Open your **Command Prompt**.

2. Start the Python interactive shell by typing:

   ```bash
   python
   ```

3. Now type the following command:

   ```python
   "   hello world   ".strip()
   ```

4. Output:

   ```
   'hello world'
   ```

### Explanation:

* The original string contains white spaces at the beginning and end.
* The `strip()` method removes **only the leading and trailing white spaces**.
* The result is a clean string: `'hello world'`.

---

## `strip()` with Specific Characters

The `strip()` method can also be used to remove **specific leading and trailing characters**. You can pass a **string of characters** as an argument to `strip()`.

### Example 1:

```python
"###hello world###".strip("#")
```

**Output:**

```
'hello world'
```

### Explanation:

* Here, we passed `"#"` as an argument.
* `strip()` removed all `#` characters from the beginning and end of the string.
* Inner characters (within the string) are **not affected**.

---

## Important Note:

* `strip()` **does not remove characters from the middle** of the string.
* It **only works from both ends** of the string—**left to right** (start) and **right to left** (end).
* It stops stripping as soon as it encounters a character **not** in the specified set.

---

## Example 2: Leading Space with Custom Character

```python
" ###hello world###".strip("#")
```

**Output:**

```
' ###hello world'
```

### Explanation:

* The first character is a **space**, not `#`.
* `strip("#")` starts at the first character. Since the space does not match `#`, it stops immediately.
* Therefore, no `#` characters are removed from the **start**.
* However, from the end, it successfully removes the trailing `#` characters.

---

## Example 3: `strip()` with Multiple Characters

You can also pass **multiple characters** as a string. Each character in that string is treated individually.

```python
"Hello world".strip("ldoH")
```

**Output:**

```
'ello wor'
```

### Explanation:

* The method removes:

  * `'H'` from the start (matches one of the given characters).
  * `'d'` and `'l'` from the end (also matches).
* As soon as it encounters a character not in `"ldoH"`, it stops.

### Case Sensitivity:

```python
"Hello world".strip("ldoh")
```

**Output:**

```
'Hello wor'
```

* Here, `'H'` is not removed because **Python is case-sensitive**.
* Only `'l'` and `'d'` at the end match and are removed.

---

## Summary

* `strip()` is used to remove **leading and trailing white spaces** by default.
* You can pass a **string of characters** to remove specific characters from both ends.
* It **does not affect characters inside** the string.
* `strip()` stops removing characters as soon as it encounters a **non-matching character** at either end.
* The method is **case-sensitive**.

---

That’s all for now on the `strip()` method. In the next session, we will explore more string methods in Python.

**Thank you for watching!**

---
