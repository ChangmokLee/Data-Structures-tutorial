# Python Data Structures Tutorial

## Introduction

Welcome to the Python Data Structures Tutorial! In this tutorial, we're going to explore the importance of data structures in programming, focusing specifically on the Stack data structure.

## Importance of Data Structures

Data structures play a crucial role in programming because they allow us to organize, manage, and store data efficiently. Understanding and using the right data structure can significantly improve the performance of our programs, making them faster and less resource-intensive.

# Data Structure 1: Stack

## Introduction to Stack

A Stack is a linear data structure that follows a particular order for performing operations: Last In First Out (LIFO). This means that the most recently added item is the first one to be removed.

## Implementing a Stack in Python

In Python, we can implement a Stack using a list or an array. The end of the list can represent the top of the stack:

\```python
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

\```

## Stack Operations

The primary operations that can be performed on a stack are:

### Push

This adds an element to the top of the stack. Here's an example of how to use the push operation in Python:

\```python
s = Stack()
s.push("Hello")
s.push("World")
print(s.stack) # Output: ['Hello', 'World']
\```

### Pop

This removes an element from the top of the stack. Here's an example of how to use the pop operation:

\```python
s = Stack()
s.push("Hello")
s.push("World")
print(s.pop()) # Output: 'World'
print(s.stack) # Output: ['Hello']
\```

### Peek

This returns the top element of the stack without removing it. Here's an example:

\```python
s = Stack()
s.push("Hello")
s.push("World")
print(s.peek()) # Output: 'World'
\```

### Size

This returns the number of elements in the stack. Here's an example:

\```python
s = Stack()
s.push("Hello")
s.push("World")
print(s.size()) # Output: 2
\```

## Conclusion

In this tutorial, we've introduced the concept of a Stack, one of the most fundamental data structures in computer science. We've implemented a Stack in Python, and we've also seen how to perform basic operations on the Stack.

Understanding Stacks is a crucial step in becoming proficient with data structures, which are vital for writing efficient code and acing technical interviews.

Keep exploring Python data structures to enhance your coding skills. In upcoming tutorials, we'll delve into other important data structures like Linked Lists and Trees.

For any further queries or assistance, feel free to reach out at lee17005@byui.edu. Stay tuned and happy coding!
