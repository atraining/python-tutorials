---
jupytext:
  text_representation:
    extension: .md
    format_name: myst
    format_version: '0.8'
    jupytext_version: 1.4.1+dev
kernelspec:
  display_name: Python 3
  language: python
  name: python3
mystnb:
  execution_timeout: 60
---

# Lists

## Introduction

In this lesson, we'll cover the basics of working with lists in Python. Lists are a versatile and commonly used data 
structure that allows you to store a collection of items, such as numbers, strings, or even other lists. We'll explore 
how to create lists, access elements, add or remove items, and perform common operations on them.

```{contents} Table of Contents
:depth: 3
```

## Creating Lists

You can create a list in Python by enclosing elements within square brackets `[ ]`, separated by commas. Let's create a 
simple list of integers:

```{code-cell}
numbers = [1, 2, 3, 4, 5]
print(numbers)
```

## Accessing Elements

You can access individual elements in a list by using their index. In Python, the index starts from 0 for the first 
element and goes up by 1 for each subsequent element. Let's access and print the second element from the list:

```{code-cell}
numbers = [1, 2, 3, 4, 5]
second_element = numbers[1]
print("The second element is:", second_element)
```

## Adding and Removing Elements

You can add elements to the end of a list using the `append()` method and remove elements using the `remove()` method. 
Let's add a new number to our existing list and then remove an element:

```{code-cell}
:tags: [remove-output]
numbers = [1, 2, 3, 4, 5]

# Adding an element
numbers.append(6)
print("After adding 6:", numbers)
```

```{code-cell}
:tags: [hide-cell]
# Removing an element
numbers.remove(3)
print("After removing 3:", numbers)
```

## List Slicing

You can extract a sublist from a list using slicing. Slicing allows you to specify a range of indices to get a portion 
of the original list. The syntax for slicing is `list[start_index:end_index]`. Let's create a new list and perform 
slicing:

```{code-cell}
numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

# Slicing to get a sublist from index 2 to 6 (exclusive)
sublist = numbers[2:6]

# Slicing to get elements from the beginning up to index 5 (exclusive)
partial_list = numbers[:5]

# Slicing to get elements from index 5 to the end
remaining_list = numbers[5:]
print("Remaining list:", remaining_list)
```

## Conclusion

Lists are incredibly useful for storing and manipulating collections of data, making them an essential part of Python 
programming. You can add and remove elements from them, as well as slice them to extract a sublist.