## **String Methods – Part 7**

In this part of our discussion on string methods, we will cover the following three important methods:

1. `count()` method
2. `find()` method
3. `rfind()` method

Let’s understand each of them one by one with examples.

---

### 🔹 **1. `count()` Method**

**Definition:**
The `count()` method returns the number of occurrences of a specified substring in a given string.

**Syntax:**

```python
string.count(sub[, start[, end]])
```

* `sub`: The substring to search for (mandatory).
* `start`: The starting index from where the search should begin (optional).
* `end`: The ending index where the search should stop (optional).

**Examples:**

```python
# Example 1
"I love fruits, fruits make me healthy".count("fruits")
# Output: 2

# Example 2 - case sensitive
"I love fruits, Fruits make me healthy".count("fruits")
# Output: 1

# Example 3 - with start and end
"I love fruits, fruits make me healthy".count("fruits", 3, 13)
# Output: 1

# Example 4 - substring not in range
"I love fruits, fruits make me healthy".count("fruits", 1, 5)
# Output: 0
```

---

### 🔹 **2. `find()` Method**

**Definition:**
The `find()` method returns the **index of the first occurrence** of a specified substring. If the substring is not found, it returns `-1`.

**Syntax:**

```python
string.find(sub[, start[, end]])
```

* `sub`: Substring to find (mandatory).
* `start`: Index to start the search (optional).
* `end`: Index to end the search (optional).

**Examples:**

```python
# Example 1 - finding a character
"Python is a beautiful language".find("b")
# Output: 12

# Example 2 - using start and end
"Python is a beautiful language".find("b", 1, 5)
# Output: -1
```

---

### 🔹 **3. `rfind()` Method**

**Definition:**
The `rfind()` method returns the **index of the last occurrence** of the specified substring. If not found, it returns `-1`.

**Syntax:**

```python
string.rfind(sub[, start[, end]])
```

* `sub`: Substring to search (mandatory).
* `start`: Start index for the search (optional).
* `end`: End index for the search (optional).

**Examples:**

```python
# Example 1
"Python is a beautiful language".rfind("e")
# Output: 29

# Example 2 - with range where substring doesn't exist
"Python is a beautiful language".rfind("e", 1, 5)
# Output: -1
```

---

### ✅ Summary

| Method    | Description                                          | Returns       |
| --------- | ---------------------------------------------------- | ------------- |
| `count()` | Counts the number of occurrences of a substring      | Integer (≥ 0) |
| `find()`  | Returns index of **first** occurrence of a substring | Index or -1   |
| `rfind()` | Returns index of **last** occurrence of a substring  | Index or -1   |

---

That concludes **Part 7** on string methods. I hope the concepts of `count()`, `find()`, and `rfind()` are now clear.
