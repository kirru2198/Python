## 📘 **Understanding `for` Loops with Dictionaries in Python**

Hello everyone, and welcome to this presentation!
In this session, we will explore how the `for` loop works with **dictionaries** in Python.

Let’s dive in without any further delay.

---

### 🔹 Topics Covered:

1. Iterating over a dictionary
2. Accessing values of a dictionary
3. Accessing keys of a dictionary
4. Accessing both keys and values of a dictionary

---

### ✅ **1. Iterating Over a Dictionary**

Just like with lists, we can use a `for` loop to iterate over a dictionary.

#### Example:

```python
course = {
    "name": "Python",
    "instructor": "Just Breath"
}

for key in course:
    print(key)
```

#### Explanation:

* The loop goes through each **key** in the `course` dictionary.
* `key` is a variable that receives one key at a time.
* The `print()` function then displays each key.

#### Output:

```
name
instructor
```

📝 **Note:** By default, iterating over a dictionary gives you the keys.

---

### ✅ **2. Accessing Values of a Dictionary**

There are two main ways to access values from a dictionary using a `for` loop:

---

#### 🔸 a. Using Square Bracket Notation

```python
for key in course:
    print(course[key])
```

#### Explanation:

* Each key is used to access the value via `course[key]`.

#### Output:

```
Python
Just Breath
```

---

#### 🔸 b. Using the `.values()` Method

```python
for value in course.values():
    print(value)
```

#### Explanation:

* `course.values()` returns a list-like view of all values in the dictionary.
* `value` gets one item at a time.

#### Output:

```
Python
Just Breath
```

📝 **Summary:**

* `course[key]` accesses values using keys.
* `course.values()` directly provides the values.

---

### ✅ **3. Accessing Keys of a Dictionary (Using `.keys()` Method)**

Although iterating directly over the dictionary gives you the keys, you can also explicitly use the `.keys()` method:

```python
for key in course.keys():
    print(key)
```

#### Output:

```
name
instructor
```

This is useful when you want to make your code more readable and explicit.

---

### ✅ **4. Accessing Both Keys and Values Using `.items()`**

To access both the **keys and values** simultaneously, use the `.items()` method.

```python
for key, value in course.items():
    print(key, value)
```

#### Explanation:

* `course.items()` returns pairs of keys and their corresponding values.
* `key` gets the key, and `value` gets the value in each iteration.

#### Output:

```
name Python
instructor Just Breath
```

📝 **Note:** The `print(key, value)` separates the two with a space by default.

---

### 🎯 Summary

| Purpose                    | Code Example                            |
| -------------------------- | --------------------------------------- |
| Iterate over keys          | `for key in course:` or `course.keys()` |
| Iterate over values        | `for value in course.values():`         |
| Access values via keys     | `course[key]`                           |
| Iterate over keys & values | `for key, value in course.items():`     |

---

### 🙏 Thank You!

This concludes our presentation on how `for` loops work with dictionaries in Python.
Thank you for watching, and I’ll see you in the next session!

---
