# Ex. No: 15C - Build a Heap Tree Using Python

## AIM:
To write a Python program to build a heap tree using appropriate Python package and function.

## ALGORITHM:

1. **Start the program.**
2. Import the `heapq` module.
3. Define a function `heaptree(H)` that takes a list `H` as input.
4. Use `heapq.heapify(H)` to convert the list into a min-heap.
5. Print the created heap.
6. **End the program.**

## PROGRAM:

```
from binarytree import heap,build,Node
def heaptree(L):
  x=L
  t=build(x)
  for i in t.values:
    print(i,"-->",end='')
  print("\nHeight : ",t.height)
  print("Is max heap? : ",t.is_max_heap)
  print("Is complete tree? : ",t.is_complete)
```

## OUTPUT
<img width="1251" height="254" alt="image" src="https://github.com/user-attachments/assets/cb42d26d-1d1a-4e9e-a8d0-125e2e737b18" />


## RESULT
Thus the Python program to build a heap tree using appropriate Python package and function has been implemented and executed successfully.
