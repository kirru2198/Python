**Presentation: How for Loop Works with Strings**

Hello everyone,
In this presentation, we will understand how to use a `for` loop with strings in Python. We will cover three main topics:

1. Accessing characters of a string using a `for` loop.
2. Iterating through a string in reverse order using a `for` loop.
3. Accessing words of a string using a `for` loop.

Let's get started!

---

### **1. Accessing Characters of a String Using a `for` Loop**

We can easily access each character of a string using a `for` loop. The loop will allow us to iterate through the string one character at a time.

---

#### **Example: Accessing Each Character in a String**

Let's say the name of a person is "John". We can access each character of this string as follows:

```python
name = "John"
for c in name:
    print(c, end=" ")
print("Done")
```

Here’s what happens:

* The variable `name` holds the string "John".
* The `for` loop iterates through each character of the string. In each iteration, the variable `c` will hold one character from the string.

  * In the first iteration, `c` will be "J".
  * In the second iteration, `c` will be "o".
  * In the third iteration, `c` will be "h".
  * In the fourth iteration, `c` will be "n".
* The `print(c, end=" ")` statement prints each character on the same line, separated by a space.

---

#### **Output**

```
J o h n Done
```

This is how you can access and display each character of a string using a `for` loop.

---

### **2. Iterating Through a String in Reverse Order Using a `for` Loop**

Now, let's explore how to access the characters of a string in reverse order using a `for` loop.

To do this, we first need to reverse the string. One way to reverse a string is through **slicing**.

---

#### **Example: Accessing Characters in Reverse Order**

Let’s use the string "John" again, but this time, we want to access the characters in reverse order:

```python
name = "John"
for c in name[::-1]:
    print(c, end=" ")
print("Done")
```

Here’s how it works:

* The slice `name[::-1]` reverses the string "John", resulting in "nhoJ".
* The `for` loop iterates through the reversed string.

  * In the first iteration, `c` will be "n".
  * In the second iteration, `c` will be "h".
  * In the third iteration, `c` will be "o".
  * In the fourth iteration, `c` will be "J".
* The `print(c, end=" ")` statement prints each character on the same line, separated by a space.

---

#### **Output**

```
n h o J Done
```

This demonstrates how to access characters of a string in reverse order using a `for` loop and slicing.

---

### **3. Accessing Words of a String Using a `for` Loop**

So far, we have accessed characters of a string. But what if we want to access words within a string?

We can use the `split()` function to split the string into words and then iterate through the resulting list of words with a `for` loop.

---

#### **Example: Accessing Words in a String**

Let’s take the sentence "Lorem ipsum dolor sit amet" and count how many words it contains:

```python
sentence = "Lorem ipsum dolor sit amet"
words = sentence.split()
count = 0

for word in words:
    count += 1

print(f"There are {count} words in the sentence.")
```

Here’s how it works:

* The `split()` function splits the string into a list of words: `["Lorem", "ipsum", "dolor", "sit", "amet"]`.
* The `for` loop iterates through each word in the list:

  * In the first iteration, `word` will be "Lorem".
  * In the second iteration, `word` will be "ipsum".
  * This continues until all the words are accessed.
* The `count` variable is incremented each time a word is accessed, allowing us to keep track of the number of words.

---

#### **Output**

```
There are 5 words in the sentence.
```

This is how you can access words in a string using a `for` loop and count the number of words.

---

### **Conclusion**

To summarize, we have learned three ways to work with strings using a `for` loop:

1. Accessing characters of a string.
2. Iterating through a string in reverse order.
3. Accessing words in a string.

These techniques are helpful when you need to process strings in Python. I hope this presentation has made these concepts clear.

Thank you for watching, and I’ll see you in the next presentation!

---
