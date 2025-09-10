# Ex. No: 15E - Expression Tree with Inorder and Postorder Traversal

## AIM:
To write a Python program to build the given expression tree and print the inorder and postorder traversals.

## ALGORITHM:

1. **Start the program.**
2. Import the required modules (`build` and `Node` from `binarytree`).
3. Define a list `x` representing the expression tree in pre-order fashion (with `None` for missing nodes).
4. Use the `build()` function to generate the binary tree.
5. Print the **inorder** and **postorder** traversal of the tree.
6. **End the program.**

## PROGRAM:

```
from binarytree import build
t = ["/","*","+","+",4,"-",2,3,1,None,None,9,5]
root = build(t)
print(root.inorder)
print(root.postorder)
```

## OUTPUT
<img width="1373" height="212" alt="image" src="https://github.com/user-attachments/assets/f1c03e69-9458-4399-bd3a-d31d4ca7c1d5" />


## RESULT
Thus the Python program to build the given expression tree and print the inorder and postorder traversals has been implemented and executed successfully.
