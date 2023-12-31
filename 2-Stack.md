# Python Data Structures Tutorial 1

## Introduction

Hello Python beginners! Welcome to this tutorial on data structures, where we'll learn about the Stack. Let's begin by understanding what a data structure is.

In computer science, a data structure is a particular way of collecting and organizing data so that we can perform operations on this data efficiently. They are the foundation of any complex programming task. In this tutorial, we're focusing on the Stack.

## What is a Stack?

A Stack is a data structure that operates on a Last In First Out (LIFO) principle. This means that the last element added is the first one to be removed.

Think about a stack of books. The last book you put on top of the stack is the first one you'll take off when you start removing books from the stack. That's how a Stack works in programming!

## Implementing a Stack in Python

In Python, we can use a built-in data structure called a list to simulate a Stack. We will define a Stack as a class, which is a blueprint for creating objects in Python.

Here is a class called Stack that we'll use to simulate a stack of items:

```python
class Stack:
def **init**(self):
self.stack = []

    def push(self, item):
        self.stack.append(item)

    def pop(self):
        if len(self.stack) < 1:
            return None
        return self.stack.pop()

    def peek(self):
        if self.stack:
            return self.stack[-1]
        return None

    def size(self):
        return len(self.stack)

```

![Example Image](media/stack.png)

## Big O Notation in Context of Stack Operations

Big O notation is a mathematical notation that describes the limiting behavior of a function when the argument tends towards a particular value or infinity. In computer science, Big O notation is used to classify algorithms according to how their run time or space requirements grow as the input size grows.

We'll now explain the Big O notation for the Stack operations as described in the code above:

- `push`: This method involves appending an item to the end of the list. In Python, this operation takes constant time, regardless of the size of the list. Therefore, the time complexity is O(1).
- `pop`: This method involves removing an item from the end of the list. Similar to the `push` method, this operation also takes constant time in Python. Therefore, the time complexity is also O(1).
- `peek`: This method involves returning the item at the end of the list without removing it. This operation also takes constant time, and therefore, its time complexity is O(1).
- `size`: This method returns the number of items in the list, which is stored as an attribute in Python lists. Therefore, this operation also has a time complexity of O(1).

In summary, all of the methods of the Stack class described above have a time complexity of O(1), which means they take a constant amount of time to execute, regardless of the size of the stack. This is one of the reasons why stacks are efficient and commonly used data structures.

## Using a Stack

Here's how we can use the Stack class to perform stack operations:

```python

# We start by creating a new Stack

s = Stack()

# We can add items to the Stack using the push method

s.push("Hello")
s.push("World")

# Printing the Stack should show that "Hello" was added first, and then "World"

print(s.stack) # Output: ['Hello', 'World']

# Removing the top item from the Stack using the pop method should return "World"

print(s.pop()) # Output: 'World'

# Printing the Stack now should show only "Hello" since "World" was removed

print(s.stack) # Output: ['Hello']

# Looking at the top item of the Stack using the peek method should return "Hello"

print(s.peek()) # Output: 'Hello'

# Finally, we can check the size of the Stack using the size method, which should return 1

print(s.size()) # Output: 1
```

![Example Image](media/stackExample2.png)

## Conclusion

And that wraps up this introduction to the Stack data structure in Python! Understanding data structures like the Stack is crucial in programming, as they can significantly improve the efficiency of your code.

In our upcoming tutorials, we will explore more fascinating data structures like Linked Lists and Trees. Keep an eye out for them!

Feel free to reach out at lee17005@byui.edu for any further queries or assistance. Happy coding!
