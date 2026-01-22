# Binary Tree – Formula Sheet
Let:
```
h = height of the tree (root at height 0)
L = number of levels = h + 1
n = total number of nodes
N₀ = number of leaf (external) nodes
N₁ = number of nodes with 1 child
N₂ = number of nodes with 2 children
```
## General Binary Tree Formulas
1. Maximum nodes at level i
```
Max nodes at level i = 2^i
```
2. Maximum nodes in a binary tree of height h
```
Max nodes = 2^(h+1) - 1
```
3. Minimum nodes in a binary tree of height h (Skewed tree case)
```
Min nodes = h + 1
```
4. Height in terms of nodes (max case)
```
h = ⌊log₂(n)⌋
```

5. Number of edges in a tree
```
Edges = n - 1
```
## Relationships Between Node Types
6. Total nodes
```
n = N₀ + N₁ + N₂
```
7. Leaf node formula (Important)
```
N₀ = N₂ + 1
```
8. Internal nodes
```
Internal nodes = N₁ + N₂
```
## Perfect / Full / Complete Binary Tree
### Perfect Binary Tree
### All levels are completely filled.

9. Total nodes
```
n = 2^(h+1) - 1
```
10. Leaf nodes
```
N₀ = 2^h
```
11. Internal nodes
```
Internal = 2^h - 1
```
## Full Binary Tree
(Each node has 0 or 2 children)

12. Total nodes
```
n = 2N₀ - 1
```
13. Leaf nodes
```
N₀ = (n + 1)/2
```
14. Internal nodes
```
Internal = (n - 1)/2
```
## Complete Binary Tree

15. Height from nodes
```
h = ⌊log₂ n⌋
```
## Binary Tree Properties

16. Minimum height for n nodes
```
h_min = ⌈log₂(n+1)⌉ - 1
```

17. Maximum height for n nodes
```
h_max = n - 1
```

18. Total number of NULL pointers in a binary tree
```
NULL pointers = n + 1
```
## Binary Search Tree (BST) Specific

19. In-order traversal of BST gives sorted order

20. Average height of BST
```
h_avg ≈ log₂ n
```

21. Worst-case height of BST
```
h_worst = n - 1
```
## Special Tree Counts

22. Number of possible binary trees with n nodes
(Catalan Number)
```
n = total nodes
C(n) = (1 / (n+1)) * (2n choose n)  ------------ (1 / (n+1)) * (2n!/n!)
```
C(3)=(1/4​)(6!/3!​)=(1/4)(20)=5 and total nodes is 3

23. Number of full binary trees with n internal nodes
```
n = internal nodes
hence  C(n) as possible binary trees but total nodes is 2n+1 
```
C(3)=(1/4​)(6!/3!​)=(1/4)(20)=5 and total nodes is 7

---
| Property                  | Formula       |
| ------------------------- | ------------- |
| Max nodes (height h)      | `2^(h+1) - 1` |
| Leaf nodes (perfect)      | `2^h`         |
| Edges                     | `n - 1`       |
| Leaf nodes in full BT     | `(n+1)/2`     |
| Internal nodes in full BT | `(n-1)/2`     |
| NULL pointers             | `n + 1`       |

---
