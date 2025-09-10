# Ex. No: 15A - Build a Binary Search Tree Using Built-in Function

## AIM:
To write a Python program to build a binary search tree using a built-in function.
## ALGORITHM:

1. **Start the program.**
2. Define `_build_bst_from_sorted_values(sorted_values)` to recursively build a binary search tree (BST) from a sorted list.
3. Define `left_subtree(l)` to print the left subtree of the BST.
4. Take user input for the number of elements and store the values in a list `a`.
5. Sort the list and pass it to `_build_bst_from_sorted_values()` to construct the BST.
6. Print the postorder traversal of the BST.
7. Call `left_subtree(l)` to print the left subtree.
8. Check whether the tree is a binary search tree using the `is_bst` property.
9. **End the program.**

## PROGRAM:

```
from binarytree import Node

# Function to build BST from sorted list using recursion
def _build_bst_from_sorted_values(sorted_values):
    if not sorted_values:
        return None
    mid = len(sorted_values) // 2
    root = Node(sorted_values[mid])
    root.left = _build_bst_from_sorted_values(sorted_values[:mid])
    root.right = _build_bst_from_sorted_values(sorted_values[mid + 1:])
    return root

# Function to print all nodes in right subtree using preorder traversal
def right_subtree(node):
    def preorder(n):
        if n:
            print(f"{n.value} -->", end="")
            preorder(n.left)
            preorder(n.right)

    print("Right Subtree :")
    preorder(node.right)
    print()

# Check if tree is BST
def is_bst(node, left=None, right=None):
    if node is None:
        return True
    if left and node.value <= left.value:
        return False
    if right and node.value >= right.value:
        return False
    return is_bst(node.left, left, node) and is_bst(node.right, node, right)

# Main block
a = []
size = int(input())
for i in range(size):
    val = int(input())
    a.append(val)

x = sorted(a)
l = _build_bst_from_sorted_values(x)

print("Postorder :", l.postorder)
right_subtree(l)
print("Is this a Binary Search Tree? ", is_bst(l))
```

## OUTPUT
<img width="1347" height="431" alt="image" src="https://github.com/user-attachments/assets/882a8532-b8aa-40a1-b8c2-4563f6b6bac3" />


## RESULT
Thus the Python program to build a binary search tree using a built-in function has been implemented and executed successfully.
