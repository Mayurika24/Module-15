# Ex. No: 15B - Build a Binary Search Tree Using Built-in Function

## AIM:
To write a Python program to build a binary search tree using a built-in function.

---

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

---

## PROGRAM:

```
from binarytree import Node
def _build_bst_from_sorted_values(sorted_values):
    
    if len(sorted_values) == 0:
        return None
    mid_index = len(sorted_values) // 2
    root = Node(sorted_values[mid_index])
    root.left = _build_bst_from_sorted_values(sorted_values[:mid_index])
    root.right = _build_bst_from_sorted_values(sorted_values[mid_index + 1 :])  
    return (root)

a=[]
size=int(input())
for i in range(0,size):
  val=int(input())
  a.append(val)
x=sorted(a)
l=_build_bst_from_sorted_values(x)
print(l.postorder)
print(l.is_bst)

```

## OUTPUT

<img width="1016" height="326" alt="image" src="https://github.com/user-attachments/assets/6f3d2aee-a9f9-4b8b-8d1d-1221d19e2e8f" />



## RESULT
Thus program Accepts float values from the user,Builds a balanced binary search tree from the sorted input list using recursion,Displays the post-order traversal of the tree,Verifies and prints whether the tree satisfies BST properties.
