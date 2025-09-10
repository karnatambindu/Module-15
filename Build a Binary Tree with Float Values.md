# Ex. No: 15B - Build a Binary Tree with Float Values

## AIM:
To write a Python program to build a binary tree with a root, left, and right node using floating-point values

## ALGORITHM:

1. **Start the program.**
2. **Import** the `Node` class from the `binarytree` module.
3. **Create a root node** using the `Node` class and assign a floating-point value.
4. **Create left and right child nodes** for the root with float values.
5. **Convert the tree** to a list and print the list of nodes.
6. **End the program.**

## PYTHON PROGRAM

```
from binarytree import Node 
l=[]
for i in range(3):
    a=input()
    l.append(a)
root=Node(l[0])
root.left=Node(l[1])
root.right=Node(l[2])
print("List of nodes :",list(root))
```

## OUTPUT
<img width="1189" height="334" alt="image" src="https://github.com/user-attachments/assets/04196598-f291-4345-b2e9-6eb976158cbc" />


## RESULT
Thus the Python program to build a binary tree with a root, left, and right node using floating-point values has been implemented and executed successfully.
