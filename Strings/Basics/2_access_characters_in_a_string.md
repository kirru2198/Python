In this presentation, we will explore how to access characters in a string in Python. Without further delay, let's dive into the topics we will cover:

1. Accessing individual characters in a string
2. Accessing individual characters from the last (negative indexing)
3. Accessing substrings of a string

Let's begin with the first topic: **Accessing Individual Characters in a String**.

### Accessing Individual Characters in a String

In Python, we can access individual characters in a string using indexing. For example, consider the string `hello`, which consists of five characters: `h`, `e`, `l`, `l`, `o`. Each character in the string is assigned a unique number, starting from `0` up to `length of the string - 1`.

In this case, the indices range from `0` to `4` (since there are 5 characters). Python uses these indices to access individual characters of the string.

Here's how to access individual characters:

```python
statement = "hello"
print(statement[0])  # Output: h
print(statement[1])  # Output: e
print(statement[2])  # Output: l
```

In this example, the first character `h` is at index `0`, the second character `e` is at index `1`, and so on.

Now, let's move on to the next topic: **Accessing Individual Characters from the Last (Negative Indexing)**.

### Accessing Individual Characters from the Last (Negative Indexing)

Python allows negative indexing to access characters starting from the end of the string. The last character of a string is assigned the index `-1`, the second-to-last character is `-2`, and so on. This feature helps us access characters without knowing the length of the string.

For example, using the string `hello`, the indices are as follows:

* `h` → index `0`, `-5`
* `e` → index `1`, `-4`
* `l` → index `2`, `-3`
* `l` → index `3`, `-2`
* `o` → index `4`, `-1`

We can access characters from the end of the string using negative indexing:

```python
statement = "hello"
print(statement[-1])  # Output: o (last character)
print(statement[-4])  # Output: e
```

This feature is particularly useful when you want to access characters from the end of a string without needing to know the exact length of the string.

Next, let's explore **Accessing Substrings of a String**.

### Accessing Substrings of a String

A substring is simply a part of a string, and Python provides a powerful feature called **slicing** to access substrings. The syntax for slicing is as follows:

```python
string[start:end]
```

Where:

* `start` is the index where the substring starts.
* `end` is the index where the substring ends (but it does not include the character at the `end` index).

For example, let's say we have the string `hello` and we want to access the substring `ell`:

```python
statement = "hello"
print(statement[1:4])  # Output: ell
```

In this example, we started at index `1` and ended at index `4`, which excludes the character at index `4`. This gives us the substring `ell`.

We can also omit the `start` index, in which case it defaults to `0`:

```python
print(statement[:4])  # Output: hell
```

In this case, the slicing starts from the beginning of the string and goes up to index `4` (excluding it), giving us the substring `hell`.

Additionally, we can use negative indexing to slice a string from the end:

```python
print(statement[-4:-1])  # Output: ell
```

This example uses negative indices to access the substring `ell`, starting from index `-4` and ending at index `-1` (excluding `-1`).

### Summary

In this presentation, we learned how to:

* Access individual characters in a string using positive indices (starting from `0`).
* Access individual characters from the last using negative indices.
* Access substrings of a string using slicing, with both positive and negative indices.

By understanding these concepts, you can efficiently work with strings and manipulate them in Python.
