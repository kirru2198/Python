# **String Formatting in Python – Part 1**

## **Introduction**

In this lesson, we will understand string formatting in Python in detail. This is **Part 1** of the topic, and we will cover three main areas:

1. What is String Formatting?
2. Percentage (%) Formatting
3. The `str.format()` Function

---

## **1. What is String Formatting?**

To understand string formatting, we first need to understand **string interpolation**. In fact, *string interpolation* and *string formatting* mean the same thing.

### **What is Interpolation?**

**Interpolation** is the process of inserting something of a different nature into something else. In simple terms, it means inserting a value into a predefined space.

### **What is String Interpolation (or String Formatting)?**

**String interpolation** is the process of inserting external values (like variables or objects) into a string. This is exactly what string formatting does—**inserts objects into a string**.

For example, if you have a string like `"My name is ____"` and you want to insert a name into it, that insertion is string interpolation.

---

## **2. Percentage (%) Formatting**

This is one of the oldest methods of string formatting in Python. Let’s look at an example using the Python interactive shell:

### **Basic Example**

```python
name = "Jaspreet"
print("My name is %s." % name)
```

* `%s` is a **placeholder** for a string.
* `% name` provides the value to insert into the placeholder.
* Output: `My name is Jaspreet.`

### **Multiple Variables**

You can use multiple placeholders:

```python
name = "Jaspreet"
city = "Delhi"
print("My name is %s and I live in %s." % (name, city))
```

* `%s` is used for strings.
* `%d` is used for integers.
* `%f` is used for floating-point numbers.

### **Example with Integers and Floats**

```python
marks = 85
percentage = 85.75
print("I got %d marks and my percentage is %f." % (marks, percentage))
```

---

## **3. The `str.format()` Function**

Python introduced a more powerful and flexible way to format strings using the `.format()` function.

### **Basic Usage**

```python
name = "Jaspreet"
city = "Delhi"
print("My name is {} and I live in {}.".format(name, city))
```

* `{}` are placeholders that will be replaced by the values passed to `.format()`.

### **Using Indexing**

You can refer to values by index:

```python
print("My name is {0} and I live in {1}.".format(name, city))
```

* `{0}` refers to the first argument (`name`)
* `{1}` refers to the second argument (`city`)

You can also switch the order:

```python
print("I live in {1} and my name is {0}.".format(name, city))
```

### **Using Keywords for Readability**

You can use keyword arguments to make strings more readable:

```python
n = "Jaspreet"
c = "Delhi"
print("My name is {name} and I live in {city}.".format(name=n, city=c))
```

### **Format Specifiers**

You can use format specifiers like `f`, `d`, and `b` inside the curly braces.

#### **Floating Point Example**

```python
print("I got {0:f} percentage marks.".format(55.66))
```

Output:

```
I got 55.660000 percentage marks.
```

#### **Using Integers as Floats**

```python
print("I got {0:f} percentage marks.".format(55))
```

Output:

```
I got 55.000000 percentage marks.
```

#### **Invalid Format**

Providing a string instead of a float:

```python
print("I got {0:f} percentage marks.".format("55"))
```

Results in:

```
ValueError: Unknown format code 'f' for object of type 'str'
```

#### **Controlling Decimal Places**

You can control how many digits appear after the decimal point using `.2f`:

```python
print("I got {0:.2f} percentage marks.".format(55.657453))
```

Output:

```
I got 55.66 percentage marks.
```

---

## **Conclusion**

In this session, we learned:

* The concept of **string formatting** or **interpolation**
* How to use **percentage (%) formatting**
* How to format strings using the **`str.format()` function**

In the next part, we will explore **f-strings**, the most modern and powerful way of string formatting in Python.

---
