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
1️⃣ Maximum nodes at level i
```
Max nodes at level i = 2^i
```
2️⃣ Maximum nodes in a binary tree of height h
```
Max nodes = 2^(h+1) - 1
```
3️⃣ Minimum nodes in a binary tree of height h
```
Min nodes = h + 1
```
(Skewed tree case)
4️⃣ Height in terms of nodes (max case)
```
h = ⌊log₂(n)⌋
```

5️⃣ Number of edges in a tree
```
Edges = n - 1
```
## Relationships Between Node Types
6️⃣ Total nodes
```
n = N₀ + N₁ + N₂
```
7️⃣ Leaf node formula (Important)
```
N₀ = N₂ + 1
```
8️⃣ Internal nodes
```
Internal nodes = N₁ + N₂
```
## Perfect / Full / Complete Binary Tree
### Perfect Binary Tree
### All levels are completely filled.

9️⃣ Total nodes
```
n = 2^(h+1) - 1
```
🔟 Leaf nodes
```
N₀ = 2^h
```
1️⃣1️⃣ Internal nodes
```
Internal = 2^h - 1
```
## Full Binary Tree
(Each node has 0 or 2 children)

1️⃣2️⃣ Total nodes
```
n = 2N₀ - 1
```
1️⃣3️⃣ Leaf nodes
```
N₀ = (n + 1)/2
```
1️⃣4️⃣ Internal nodes
```
Internal = (n - 1)/2
```
## Complete Binary Tree

1️⃣5️⃣ Height from nodes
```
h = ⌊log₂ n⌋
```
## Binary Tree Properties

1️⃣6️⃣ Minimum height for n nodes
```
h_min = ⌈log₂(n+1)⌉ - 1
```

1️⃣7️⃣ Maximum height for n nodes
```
h_max = n - 1
```

1️⃣8️⃣ Total number of NULL pointers in a binary tree
```
NULL pointers = n + 1
```
## Binary Search Tree (BST) Specific

1️⃣9️⃣ In-order traversal of BST gives sorted order

2️⃣0️⃣ Average height of BST
```
h_avg ≈ log₂ n
```

2️⃣1️⃣ Worst-case height of BST
```
h_worst = n - 1
```
## Special Tree Counts

2️⃣2️⃣ Number of possible binary trees with n nodes
(Catalan Number)
```
C(n) = (1 / (n+1)) * (2n choose n)
```

2️⃣3️⃣ Number of full binary trees with n internal nodes
```
= C(n)
```
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
