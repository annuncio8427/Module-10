# Stack Implementation Using `LifoQueue` (Max Size 7) 🔄

This Python program demonstrates a stack implemented using the `LifoQueue` class from the `queue` module. It allows up to 7 elements, checks if the stack is full, and then prints the elements in reverse (LIFO) order.

## 🎯 Aim

To create a Python program that:
- Implements a stack using `LifoQueue` with a maximum size of 7
- Adds user-inputted values to the stack
- Checks whether the stack is full
- Prints the stack elements in reverse order (LIFO)

## 📋 Algorithm

1. Import the `LifoQueue` class from the `queue` module.
2. Create a stack with a maximum size of 7.
3. Read the number of elements (`n`) to be added to the stack.
4. Loop `n` times:
   - Read a value from the user.
   - Use `put()` to push it onto the stack if it's not full.
5. Use `full()` to check if the stack is full and print the result.
6. Use `get()` repeatedly to pop and print elements in reverse order.

## Program

from queue import LifoQueue

stack = LifoQueue(maxsize=7)

n = int(input())
for i in range(n):
    value = input()
    if not stack.full():
        stack.put(value)

if stack.full():
    print("Stack is full")
else:
    print("Stack is not full")

print("Stack elements in LIFO order:")
while not stack.empty():
    print(stack.get())


## 🧪 Sample Input and Output

Input:
5
apple
orange
grape
banana
melon

Output:
Stack is not full
Stack elements in LIFO order:
melon
banana
grape
orange
apple


## Result:

The program successfully:

Implements a stack using LifoQueue with a maximum size of 7

Accepts and stores user input values

Checks whether the stack is full or not

Removes and prints the elements in LIFO (reverse) order
