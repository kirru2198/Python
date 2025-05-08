# Python String Slicing – Negative Third Parameter & Reversing a String

Welcome! In this session, we will continue our discussion on **string slicing in Python**. Specifically, we'll cover:

1. **Negative Third Parameter** in slicing
2. **Reversing a String** using slicing

Let's get started.

---

## 🔁 Recap: The Third Parameter in Slicing

In Python, string slicing follows the syntax:

```python
string[start:stop:step]
```

* **start**: Index to begin the slice (inclusive)
* **stop**: Index to end the slice (exclusive)
* **step**: Also called the **step value**, it tells Python **how many characters to skip** at each step.

By default, `step` is `+1`, meaning no characters are skipped and the string is read **left to right**.

---

## 📉 Understanding Step Value

If you specify a positive step (e.g., `2`), Python skips every `(step - 1)` character.
For example:

```python
s = "I am just breathe"
print(s[0:8:2])
```

**Explanation:**

* `start = 0`, `stop = 8`, `step = 2`
* Characters read: `s[0]`, skip one, `s[2]`, skip one, `s[4]`, skip one, `s[6]`
* Result: `'Ia a'`

---

## 🔄 Negative Step (Reversing Direction)

When the **step value is negative**, Python reads the string **right to left**.

### Example:

```python
s = "I am just breathe"
print(s[8:1:-2])
```

**Explanation:**

* `start = 8` → character `'p'`
* `stop = 1` → slicing will stop **before** index 1
* `step = -2` → move two steps backward each time (i.e., skip one character backward)
* Characters read: `s[8]` (`'p'`), `s[6]` (`'a'`), `s[4]` (`' '`), `s[2]` (`'a'`)
* Result: `'pa a'`

### Key Observations:

1. Negative step means reading from **right to left**
2. The **start index** must be **greater** than the **stop index**
3. To compute the number of elements to skip:

   * For positive steps: skip = `step - 1`
   * For negative steps: skip = `abs(step) - 1`

---

## 🔁 Reversing a String with Negative Step

To reverse an entire string using slicing, simply set the step to `-1`:

```python
s = "I am just breathe"
print(s[::-1])
```

**Output:** `'htaerb tsuj ma I'`

You can also try:

```python
s = "string"
print(s[::-1])
```

**Output:** `'gnirts'`

This technique works because:

* Start and stop are omitted → entire string is considered
* Step is `-1` → string is read from last to first character

---

## 🧠 Another Example

Let's look at:

```python
s = "string"
print(s[5:0:-1])
```

**Explanation:**

* `start = 5` → character `'g'`
* `stop = 0` → slicing stops **before index 0**
* `step = -1` → read in reverse order
* Result: `'gnirt'` (characters at indices `5, 4, 3, 2, 1`)

If you want to include the character at index `0`, update the stop index to `-1`:

```python
print(s[5::-1])  # Output: 'gnirts'
```

---

## ✅ Summary: Negative Third Parameter in Slicing

| Concept                   | Description                |
| ------------------------- | -------------------------- |
| **Direction**             | Right to left              |
| **Step Value**            | Must be negative           |
| **Start > Stop**          | Required for negative step |
| **Skip Count**            | `abs(step) - 1`            |
| **Reverse Entire String** | `s[::-1]`                  |

---

## 🏁 Final Thoughts

You’ve now learned:

* How slicing works with a **negative step value**
* How to **reverse strings** using slicing in Python
* The **importance of choosing correct start, stop, and step values** based on slicing direction

This is a powerful and concise feature of Python for string manipulation. Practice these examples to reinforce your understanding.

---
