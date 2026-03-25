# Ex. No: 15E - Build and Evaluate an Expression Tree

## AIM:
To write a Python program to build and evaluate the given Expression tree.

---

## ALGORITHM:

1. **Start the program.**
2. Create nodes for operators and operands.
3. Build the expression tree by connecting nodes in the correct hierarchical structure.
4. Define a recursive function `evaluate(root)`:
   - If the node is a number (leaf), return it.
   - Else, recursively evaluate left and right subtrees.
   - Apply the operator at the current node to the results.
5. Return the final result from the root node.
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

## OUTPUT:
<img width="1024" height="104" alt="image" src="https://github.com/user-attachments/assets/4ac7d256-636d-41f2-a44e-1cba5d72e28e" />


## RESULT:
Thus the program succesffuly completed the Build an Expression Tree and Print Inorder and Postorder Traversals and executrd successfully.
