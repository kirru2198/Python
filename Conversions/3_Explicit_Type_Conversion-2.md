## 🎓 **Explicit Type Conversion in Python - Part 2**

Welcome to **Part 2** of our discussion on **Explicit Type Conversion in Python**. In the previous session, we covered the basics of explicit type conversion and specifically looked at the `int()` function. Today, we will explore more functions for type conversion, focusing on **float** and **str**.

Let’s dive into today’s topics:

1. **Explicit Type Conversion Using `float`**
2. **Explicit Type Conversion Using `str`**
3. **Homework Problem and Error Rectification**

---

### 🧪 **Explicit Type Conversion Using `float`**

Explicit type conversion using `float` refers to converting a value from one data type to a **floating-point number** through user intervention.

The syntax for using `float()` is simple:

```python
float(value)
```

Where `value` is the object that you want to convert into a floating-point number. Let’s see some examples:

---

#### **Example 1: Converting an Integer to Float**

```python
x = 78
x = float(x)
print(x)  # Output: 78.0
```

In this example, we convert the integer `78` into a floating-point number `78.0`. Notice how the result is automatically converted to float.

---

#### **Example 2: Converting a String to Float**

```python
y = '3.14159'
y = float(y)
print(y)  # Output: 3.14159
```

Here, we convert the string `'3.14159'` to a floating-point number `3.14159`.

---

#### **Example 3: Removing Leading Zeros in a String Representation of a Float**

```python
z = '0078.90'
z = float(z)
print(z)  # Output: 78.9
```

In this case, the string `'0078.90'` is converted into the floating-point number `78.9`, with the leading zeros automatically discarded.

---

### 🔄 **Summary of `float()` Conversion**

* **`float()`** converts both integers and strings to floating-point numbers.
* It removes any non-significant zeros from floating-point strings.
* It’s important to note that `float()` can also handle numerical strings (e.g., `'3.14'`).

---

### 🧪 **Explicit Type Conversion Using `str`**

Next, let's discuss **explicit type conversion using `str()`**. The `str()` function converts a value of any data type into a **string**.

The syntax for using `str()` is as follows:

```python
str(value)
```

Where `value` is the object you want to convert to a string. Let’s look at some examples:

---

#### **Example 1: Converting an Integer to String**

```python
x = 198
x = str(x)
print(x)  # Output: '198'
```

In this case, the integer `198` is successfully converted into the string `'198'`.

---

#### **Example 2: Verifying the Type of the Converted Value**

To verify that the conversion has been successful, we can use the `type()` function:

```python
print(type(x))  # Output: <class 'str'>
```

This confirms that `x` is now a string.

---

### 🔄 **Summary of `str()` Conversion**

* **`str()`** converts an object of any type (integer, float, etc.) into a string.
* The conversion is useful when you need to perform string concatenation or manipulation with other data types.

---

### 📝 **Homework Problem**

Let’s now revisit the homework problem from this session. Here is the code:

```python
x = 10
y = 20
total = x + y
print("The total is: " + total)
```

#### **Error Explanation:**

This code throws the following error:

```
TypeError: can only concatenate str (not "int") to str
```

#### **Error Cause:**

The error occurs because the `+` operator is used to concatenate the string `"The total is: "` with the integer `total`, which results in a **TypeError**. Python does not allow implicit conversion of an integer to a string for concatenation.

#### **Solution:**

To fix this error, we need to explicitly convert the integer `total` to a string using the `str()` function. The corrected code should look like this:

```python
x = 10
y = 20
total = x + y
print("The total is: " + str(total))
```

This ensures that `total` is converted to a string before concatenation, and the program will run without errors.

---

### 📚 **Conclusion**

* **Explicit Type Conversion** allows the programmer to manually convert one type of object to another using functions like `float()` and `str()`.
* We learned how to use **`float()`** to convert values to floating-point numbers and **`str()`** to convert values to strings.
* Finally, we worked through a **homework problem** and rectified the error by explicitly converting the integer to a string.

---
