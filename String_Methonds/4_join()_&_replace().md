# **Introduction to String Methods**

In this session, we will learn about two important string methods in Python:

1. **`join()` Method**
2. **`replace()` Method**

After discussing both methods with examples, we will look at a few **homework problems** to test our understanding.

---

## **1. `join()` Method**

### **Purpose**

The `join()` method is used to **combine the elements of an iterable** into a single string. You specify a **separator**, and it inserts that between each element of the iterable.

### **Syntax**

```python
separator.join(iterable)
```

### **What is an Iterable?**

An **iterable** is an object that can return its members one at a time. Examples of iterables include:

* Strings
* Lists
* Tuples
* Dictionaries
* Sets

You can iterate over each element in an iterable using loops or functions like `join()`.

---

### **Examples with `join()`**

#### **Example 1: Join Characters in a List**

```python
L1 = ['h', 'e', 'l', 'l', 'o']
''.join(L1)
# Output: 'hello'
```

Here, an empty string is used as the separator.

#### **Example 2: Join Words with Space**

```python
L2 = ['I', 'am', 'Rocky']
' '.join(L2)
# Output: 'I am Rocky'
```

#### **Example 3: Join with Underscore**

```python
L3 = ['name', 'of', 'a', 'variable']
'_'.join(L3)
# Output: 'name_of_a_variable'
```

#### **Example 4: Join Dictionary Keys**

```python
d = {'name': 'Adam', 'country': 'US'}
' and '.join(d)
# Output: 'name and country'
```

> Note: When you pass a dictionary to `join()`, only the **keys** are joined, not the values.

---

## **2. `replace()` Method**

### **Purpose**

The `replace()` method is used to **replace a substring with another substring** within a string.

### **Syntax**

```python
string.replace(old, new, count)
```

* `old`: The substring you want to replace.
* `new`: The substring to replace it with.
* `count` *(optional)*: The number of occurrences to replace. If not provided, all instances are replaced.

---

### **Examples with `replace()`**

#### **Example 1: Simple Replacement**

```python
s = "I love to eat strawberries"
s.replace("strawberries", "mangoes")
# Output: 'I love to eat mangoes'
```

#### **Example 2: Replace Limited Occurrences**

```python
s = "I love to eat strawberries"
s.replace(" ", "-", 2)
# Output: 'I-love-to eat strawberries'
```

> Only the **first two spaces** are replaced with hyphens.

#### **Example 3: Replace All Occurrences**

```python
s = "I love to eat strawberries"
s.replace(" ", "-")
# Output: 'I-love-to-eat-strawberries'
```

---

## **Homework Problems**

### **Problem 1: Output Prediction**

```python
s = "I love to eat strawberries"
print(s.replace("strawberries", "mangoes"))
```

> What will be the output?

---

### **Problem 2: Join Integers in a List**

```python
L = [1, 2]
''.join(L)
```

> Will this work? Answer with **Yes** or **No**.

> Hint: The `join()` method works only with **strings**, not integers. You would first need to convert each integer to a string using `str()`.

---

## **Summary**

* The `join()` method is used to combine elements of an iterable using a separator.
* The `replace()` method replaces occurrences of a substring within a string.
* Both methods are very useful for string manipulation in Python.

---

Thank you for following along! See you in the next session.
