# Ex. No: 15C - Expression Tree with Inorder and Postorder Traversal

## AIM:
To write a Python program to build the given expression tree and print the inorder and postorder traversals.

---

## ALGORITHM:

1. **Start the program.**
2. Import the required modules (`build` and `Node` from `binarytree`).
3. Define a list `x` representing the expression tree in pre-order fashion (with `None` for missing nodes).
4. Use the `build()` function to generate the binary tree.
5. Print the **inorder** and **postorder** traversal of the tree.
6. **End the program.**

---

## PROGRAM:

```
from binarytree import build

l=["*","+","-",9,3,8,4]
bt=build(l)
print(bt.inorder)
print(bt.postorder)
```

## OUTPUT
<img width="1024" height="104" alt="image" src="https://github.com/user-attachments/assets/8c2196d5-6af0-4782-9d65-8cd3c921c370" />

## RESULT
Thus the program succesffuly completed the Build an Expression Tree and Print Inorder and Postorder Traversals and executrd successfully.
