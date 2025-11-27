# Queue-Queue Values in Descending Order Using Python 🧮

This Python program simulates a queue using a list, removes the first two elements (FIFO order), and displays the remaining values in descending order.

## 🎯 Aim

To write a Python program to:
- Accept user inputs into a list (queue)
- Remove the first two elements (simulating dequeue)
- Display the remaining values in **descending order**

## 🧠 Algorithm

1. Create an empty list `q`.
2. Read an integer `n` to determine how many elements will be added.
3. Loop `n` times:
   - Read an input value.
   - Append it to the list `q`.
4. Remove the first element using `pop(0)`.
5. Remove the second element using `pop(0)` again.
6. Sort the list in descending order.
7. Print the updated list.

## 🧪 Program:

```python
q = []
n = int(input())
for i in range(n):
    value = int(input())
    q.append(value)
q.pop(0)
q.pop(0)
q.sort(reverse=True)
print(q)
```

### Output:

**Input:**
```
5
10
40
20
60
30
```

**Output:**
```
[60, 40, 30]
```

## Result:

The program successfully removes the first two elements from the queue and displays the remaining values in descending order.
