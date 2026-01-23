# DSA Notes 
<pre>
  
                      📘 1. Data Structures and Algorithms (DSA)
                      Description:
                      DSA is a foundational subject in computer science that combines data structures (ways to organize data) and algorithms (procedures to process data). Mastering DSA improves problem-solving and coding efficiency.
                      Main Points:
                      •	Data Structures: Organize and store data efficiently.
                      •	Algorithms: Step-by-step methods to solve problems.
                      •	Crucial for coding interviews and system performance.
                      •	Used in real-world applications like databases, operating systems, etc.
                      Simple Example:
                      // Algorithm to find the maximum number in an array
                      function findMax(arr) {
                      let max = arr[0];
                      for (let i = 1; i < arr.length; i++) {
                        if (arr[i] > max) {
                          max = arr[i];
                        }
                      }
                      return max;
                      }
                      ________________________________________
                      📘 2. What is Data Structure?
                      Description:
                      A data structure is a specific format to organize, manage, and store data for efficient access and modification.
                      Main Points:
                      •	Types: Linear (Arrays, Linked Lists) and Non-linear (Trees, Graphs)
                      •	Helps in faster data operations: insertion, deletion, searching, sorting
                      •	Choice of data structure affects performance
                      Simple Example:
                      // Using an array to store and access data
                      let fruits = ['Apple', 'Banana', 'Cherry'];
                      console.log(fruits[1]); // Output: Banana
                      ________________________________________
                      📘 3. What is an Algorithm?
                      Description:
                      An algorithm is a step-by-step set of instructions to perform a task or solve a problem.
                      Main Points:
                      •	Must be clear, finite, and effective
                      •	Input → Process → Output
                      •	Examples: Sorting, Searching, Traversal
                      •	Evaluated based on time and space efficiency
                      Simple Example:
                      // Algorithm to check if a number is even or odd
                      function isEven(num) {
                      return num % 2 === 0;
                      }
                      ________________________________________
                      📘 4. Asymptotic Notation
                      Description:
                      Asymptotic Notation describes the performance (time or space) of an algorithm as the input size grows. It helps analyze algorithm efficiency without running code.
                      Main Points:
                      •	Big O (O) – Worst case
                      •	Omega (Ω) – Best case
                      •	Theta (Θ) – Average case
                      •	Focuses on scalability and efficiency
                      Simple Example:
                      // O(n) - Linear time example
                      function printItems(arr) {
                      for (let item of arr) {
                        console.log(item);
                      }
                      }
                      ________________________________________
                      📘 5. Pointer in Data Structure
                      Description:
                      A pointer is a variable that stores the memory address of another variable. It's heavily used in dynamic memory allocation and data structures like linked lists.
                      Main Points:
                      •	Points to memory location
                      •	Used in C/C++, not in JavaScript
                      •	Crucial for linked structures (like Linked List, Tree)
                      •	Enables dynamic memory management
                      Simple Example (C language):
                      int a = 10;
                      int *p = &a;
                      printf("%d", *p); // Output: 10
                      ________________________________________
                      📘 6. Abstract Data Type (ADT) in Data Structure
                      Description:
                      An ADT is a logical description of how data is viewed and the operations allowed, without specifying how it is implemented.
                      Main Points:
                      •	Focuses on what operations are to be performed
                      •	Examples: Stack, Queue, List, Set, Map
                      •	Helps in abstraction and encapsulation
                      •	Implementation can vary (Array, Linked List, etc.)
                      Simple Example:
                      // Stack ADT behavior using array
                      let stack = [];
                      stack.push(10);
                      stack.push(20);
                      console.log(stack.pop()); // Output: 20
                      ________________________________________
                      📘 7. DS Array
                      Description:
                      In Data Structures (DS), an Array is a linear data structure that stores elements of the same type in contiguous memory locations and allows fast access using indices.
                      Main Points:
                      •	Fixed size and static memory allocation
                      •	Zero-based indexing
                      •	Fast random access: O(1) time for accessing elements
                      •	Insertion/deletion can be expensive due to shifting
                      Simple Example:
                      let numbers = [10, 20, 30, 40];
                      console.log(numbers[2]); // Output: 30
                      ________________________________________
                      📘 8. Multidimensional Array
                      Description:
                      A Multidimensional Array is an array with more than one index, typically used to represent matrices, tables, or grids.
                      Main Points:
                      •	Common form: 2D arrays (rows × columns)
                      •	3D or more dimensions used for simulations or image data
                      •	Accessed via multiple indices
                      •	Stored in row-major or column-major order in memory (language-dependent)
                      Simple Example (2D in C++):
                      int matrix[2][3] = {
                      {1, 2, 3},
                      {4, 5, 6}
                      };
                      cout << matrix[1][2]; // Output: 6
                      ________________________________________
                      📘 9. Sparse Matrix
                      Description:
                      A Sparse Matrix is a matrix in which most of the elements are zero. Instead of storing all elements, only non-zero values are stored to optimize space and performance.
                      Main Points:
                      •	Reduces memory usage
                      •	Used in scientific computing, ML, and graphs
                      •	Representations: Triplet Format, Dictionary of Keys (DOK), CSR (Compressed Sparse Row)
                      •	Can speed up computations on large matrices
                      Simple Example (Triplet Representation):
                      // [row, col, value]
                      let sparse = [
                      [0, 3, 5],
                      [1, 0, 8],
                      [2, 2, 6]
                      ];
                      // Represents non-zero entries of a 3x4 matrix
                      ________________________________________
                      📘 10. Advantages of Using Arrays
                      Description:
                      Arrays are a foundational data structure offering fast, indexed access and are supported in virtually all programming languages.
                      Main Points:
                      •	Fast element access using indices (O(1))
                      •	Easy to traverse using loops
                      •	Simplicity and wide usage
                      •	Ideal for fixed-size, homogeneous data
                      •	Works well with CPU caching due to contiguous memory layout
                      Simple Example:
                      let colors = ['red', 'green', 'blue'];
                      console.log(colors[0]); // Output: red
                      ________________________________________
                      📘 11. DS Linked List
                      Description:
                      A Linked List is a linear data structure where elements (nodes) are connected using pointers. Unlike arrays, elements are not stored in contiguous memory.
                      Main Points:
                      •	Each node contains: data + pointer to the next (and/or previous) node
                      •	Dynamic size — efficient insertions/deletions
                      •	No random access (unlike arrays)
                      •	Used in memory management, stacks, queues, etc.
                      Simple Example (Singly Linked List Node in C):
                      struct Node {
                        int data;
                        struct Node* next;
                      };
                      ________________________________________
                      📘 12. Linked List in Data Structure
                      Description:
                      A Linked List allows elements to be linked together using pointers, forming a chain-like structure that can grow or shrink during runtime.
                      Main Points:
                      •	Nodes are stored anywhere in memory
                      •	No need to define size beforehand
                      •	Types: Singly, Doubly, Circular, Circular Doubly
                      •	Useful for implementing dynamic memory-based data structures
                      Simple Example (Traversal in JavaScript-like syntax):
                      class Node {
                      constructor(data) {
                        this.data = data;
                        this.next = null;
                      }
                      }
                      
                      let head = new Node(10);
                      head.next = new Node(20);
                      console.log(head.next.data); // Output: 20
                      ________________________________________
                      📘 13. Types of Linked List
                      Description:
                      There are several types of Linked Lists, each with different pointer configurations to optimize access and traversal.
                      Main Points:
                      •	Singly Linked List – Nodes point to next node only
                      •	Doubly Linked List – Nodes point to both next and previous
                      •	Circular Linked List – Last node links back to head
                      •	Circular Doubly Linked List – Combines doubly and circular features
                      Simple Diagram (Conceptual):
                      Singly:    A -> B -> C -> NULL  
                      Doubly:    NULL <- A <-> B <-> C -> NULL  
                      Circular:  A -> B -> C -> A  
                      ________________________________________
                      📘 14. Singly Linked List
                      Description:
                      A Singly Linked List is a type of linked list where each node contains data and a pointer to the next node only.
                      Main Points:
                      •	Unidirectional traversal
                      •	Simpler to implement
                      •	Used in stacks, basic list structures
                      •	Cannot traverse backwards
                      Simple Example:
                      class Node {
                      constructor(data) {
                        this.data = data;
                        this.next = null;
                      }
                      }
                      let head = new Node(1);
                      head.next = new Node(2);
                      ________________________________________
                      📘 15. Doubly Linked List
                      Description:
                      A Doubly Linked List allows traversal in both directions as each node has two pointers: one for the next node and one for the previous.
                      Main Points:
                      •	Bidirectional navigation
                      •	More complex, but more flexible
                      •	Used in navigation systems, undo/redo, and memory-efficient applications
                      •	Extra memory used for previous pointer
                      Simple Example:
                      class Node {
                      constructor(data) {
                        this.data = data;
                        this.prev = null;
                        this.next = null;
                      }
                      }
                      ________________________________________
                      📘 16. Circular Linked List
                      Description:
                      A Circular Linked List is a list in which the last node points back to the first node, forming a loop.
                      Main Points:
                      •	No NULL at the end
                      •	Useful in circular queues and buffers
                      •	Can be singly or doubly circular
                      •	Infinite traversal risk if not handled carefully
                      Simple Example (conceptual):
                      head.next.next.next = head; // Last node links to head
                      ________________________________________
                      📘 17. Circular Doubly Linked List
                      Description:
                      A Circular Doubly Linked List is a list where each node has both next and previous pointers, and the last node connects back to the first.
                      Main Points:
                      •	Combines advantages of doubly and circular lists
                      •	Traversable in both directions infinitely
                      •	Used in scheduling algorithms (e.g., round-robin), multimedia players
                      Simple Example (logic):
                      node1.prev = node3;
                      node3.next = node1; 
                      
                      📘 18. DS Stack
                      Description:
                      A Stack is a linear data structure that follows the LIFO (Last In, First Out) principle — the last element added is the first one to be removed.
                      Main Points:
                      •	Operations: push (insert), pop (remove), peek (view top)
                      •	LIFO behavior
                      •	Used in function calls, undo features, syntax parsing
                      •	Can be implemented using arrays or linked lists
                      Simple Example:
                      let stack = [];
                      stack.push(10);
                      stack.push(20);
                      console.log(stack.pop()); // Output: 20
                      ________________________________________
                      📘 19. Stack in Data Structure
                      Description:
                      In DS, a Stack stores elements in a controlled order using restricted operations — only the top element is accessible at any time.
                      Main Points:
                      •	Access is limited to the top
                      •	Used to reverse elements or maintain order
                      •	Memory-efficient for last-in-first-out use cases
                      •	Overflow and underflow must be handled in fixed-size implementations
                      Simple Example:
                      // Simulating call stack
                      function greet() {
                      console.log("Hello");
                      }
                      function start() {
                      greet();
                      }
                      start(); // Stack: start() → greet() → print
                      ________________________________________
                      📘 20. Implementation of Stack using Array
                      Description:
                      A stack can be implemented using an array by keeping track of the top index.
                      Main Points:
                      •	Simple and fast if size is known
                      •	Risk of overflow if size limit is exceeded
                      •	push: top++, pop: top--
                      Simple Example (in C++):
                      int stack[100], top = -1;
                      
                      void push(int val) {
                        stack[++top] = val;
                      }
                      
                      int pop() {
                        return stack[top--];
                      }
                      ________________________________________
                      📘 21. Implementation of Stack using Linked List
                      Description:
                      A Linked List-based stack dynamically allocates memory, making it flexible with no fixed size.
                      Main Points:
                      •	No size limit (dynamic memory)
                      •	Each push creates a new node at the head
                      •	Pop removes the head node
                      Simple Example (in C):
                      struct Node {
                        int data;
                        struct Node* next;
                      };
                      
                      void push(struct Node** top, int val) {
                        struct Node* newNode = malloc(sizeof(struct Node));
                        newNode->data = val;
                        newNode->next = *top;
                        *top = newNode;
                      }
                      ________________________________________
                      📘 22. Application of Stack in Data Structure
                      Description:
                      Stacks are used in many real-world and system-level applications due to their LIFO behavior.
                      Main Points:
                      •	Function call and recursion stack
                      •	Undo/Redo in text editors
                      •	Expression evaluation (postfix, prefix)
                      •	Syntax parsing in compilers
                      •	Balanced parenthesis checking
                      Simple Example: Balanced Parentheses
                      function isBalanced(expr) {
                      let stack = [];
                      for (let char of expr) {
                        if (char === '(') stack.push(char);
                        else if (char === ')') {
                          if (!stack.length) return false;
                          stack.pop();
                        }
                      }
                      return stack.length === 0;
                      }
                      console.log(isBalanced("(a+b)*(c-d)")); // true
                      ________________________________________
                      📘 23. DS Queue
                      Description:
                      A Queue is a linear data structure that follows the FIFO (First In, First Out) principle — the first element added is the first one to be removed.
                      Main Points:
                      •	Operations: enqueue (insert), dequeue (remove)
                      •	FIFO behavior
                      •	Used in scheduling, buffering, and messaging systems
                      •	Can be implemented using arrays or linked lists
                      Simple Example:
                      let queue = [];
                      queue.push(10);       // enqueue
                      queue.push(20);
                      console.log(queue.shift()); // dequeue → Output: 10
                      ________________________________________
                      📘 24. Queue in Data Structure
                      Description:
                      A Queue is used to manage elements in the order they arrive. It allows insertion at the rear and deletion from the front.
                      Main Points:
                      •	Maintains order of processing
                      •	Static (array-based) or dynamic (linked list-based)
                      •	Linear and easy to implement
                      •	Overflow and underflow must be handled
                      Simple Example:
                      let queue = [1, 2, 3];
                      queue.push(4); // enqueue
                      queue.shift(); // dequeue (removes 1)
                      ________________________________________
                      📘 25. Types of Queues
                      Description:
                      There are various specialized queues designed for different scenarios.
                      Main Points:
                      •	Simple Queue: FIFO queue
                      •	Circular Queue: Last position connects to the first
                      •	Priority Queue: Elements served based on priority
                      •	Double Ended Queue (Deque): Insertion/deletion from both ends
                      Simple Diagram:
                      Simple Queue:  Front → A B C D ← Rear  
                      Circular Queue: D connects back to A  
                      ________________________________________
                      📘 26. Implementation of Queue using Array
                      Description:
                      A simple queue can be implemented using an array with front and rear indices.
                      Main Points:
                      •	Easy to implement
                      •	Fixed size (risk of overflow)
                      •	Front is updated on dequeue, rear on enqueue
                      Simple Example (C++):
                      int queue[100], front = -1, rear = -1;
                      
                      void enqueue(int val) {
                        if (rear == 99) return;
                        if (front == -1) front = 0;
                        queue[++rear] = val;
                      }
                      
                      int dequeue() {
                        return (front > rear) ? -1 : queue[front++];
                      }
                      ________________________________________
                      📘 27. Implementation of Queue using Linked List
                      Description:
                      In this approach, each node holds data and a pointer to the next. The queue maintains pointers to front and rear.
                      Main Points:
                      •	No size limit
                      •	Dynamic memory allocation
                      •	Efficient for continuous enqueue/dequeue
                      Simple Example (C):
                      struct Node {
                        int data;
                        struct Node* next;
                      };
                      
                      struct Node *front = NULL, *rear = NULL;
                      
                      void enqueue(int val) {
                        struct Node* newNode = malloc(sizeof(struct Node));
                        newNode->data = val;
                        newNode->next = NULL;
                        if (rear == NULL) front = rear = newNode;
                        else {
                            rear->next = newNode;
                            rear = newNode;
                        }
                      }
                      ________________________________________
                      📘 28. Circular Queue
                      Description:
                      A Circular Queue reuses the empty space in an array by connecting the rear to the front, making the queue wrap around.
                      Main Points:
                      •	Avoids false overflow
                      •	Rear and front move circularly using modulo
                      •	Efficient memory utilization
                      Simple Example (Logic):
                      rear = (rear + 1) % size;
                      front = (front + 1) % size;
                      ________________________________________
                      📘 29. Priority Queue
                      Description:
                      A Priority Queue serves elements based on priority rather than insertion order.
                      Main Points:
                      •	Higher priority served first (not FIFO)
                      •	Can be implemented using arrays, heaps, or linked lists
                      •	Used in CPU scheduling, Dijkstra’s algorithm, etc.
                      Simple Example (Concept):
                      let pq = [
                      { value: 'A', priority: 2 },
                      { value: 'B', priority: 1 }
                      ];
                      pq.sort((a, b) => a.priority - b.priority);
                      console.log(pq.shift()); // Output: B
                      ________________________________________
                      📘 30. Double Ended Queue (Deque)
                      Description:
                      A Deque allows insertion and deletion at both ends — front and rear.
                      Main Points:
                      •	More flexible than a regular queue
                      •	Types: Input-restricted and output-restricted
                      •	Used in palindrome checking, sliding window problems
                      Simple Example (JavaScript):
                      let deque = [];
                      deque.push(10);       // insert rear
                      deque.unshift(5);     // insert front
                      deque.pop();          // remove rear
                      deque.shift();        // remove front
                      ________________________________________
                      📘 31. Application of Queue in Data Structure
                      Description:
                      Queues are used in a wide range of real-time and system-level tasks requiring ordered processing.
                      Main Points:
                      •	CPU task scheduling (Round Robin)
                      •	Print queues in printers
                      •	Breadth-first search (BFS) in graphs
                      •	Call center/customer service queue
                      •	Data buffers in streaming
                      Simple Example: BFS (Queue used in traversal):
                      function BFS(graph, start) {
                      let visited = new Set();
                      let queue = [start];
                      while (queue.length) {
                        let node = queue.shift();
                        if (!visited.has(node)) {
                          visited.add(node);
                          queue.push(...graph[node]);
                        }
                      }
                      }
                      ________________________________________
                      📘 32. DS Tree
                      Description:
                      A Tree is a non-linear hierarchical data structure where elements are arranged in a parent-child relationship.
                      Main Points:
                      •	Consists of nodes and edges
                      •	Root: topmost node
                      •	Leaf: node with no children
                      •	Recursive structure: each subtree is itself a tree
                      •	Used in hierarchical data, databases, compilers
                      Simple Example (Structure):
                            A
                           / \
                          B   C
                         / \
                        D   E
                      ________________________________________
                      📘 33. Tree (Data Structure)
                      Description:
                      A Tree organizes data in levels and sublevels, ideal for representing hierarchies (like file systems or XML/HTML documents).
                      Main Points:
                      •	Tree Traversals: Preorder, Inorder, Postorder, Level-order
                      •	Types: Binary Tree, Binary Search Tree, Balanced Trees, etc.
                      •	No cycles (unlike graphs)
                      •	One node is the root; every node has one parent (except root)
                      Simple Example (Inorder traversal - Left, Root, Right):
                      function inorder(node) {
                      if (node !== null) {
                        inorder(node.left);
                        console.log(node.value);
                        inorder(node.right);
                      }
                      }
                      ________________________________________
                      📘 34. Binary Tree
                      Description:
                      A Binary Tree is a tree where each node has at most two children, referred to as left and right.
                      Main Points:
                      •	Perfect Binary Tree: all levels full
                      •	Complete Binary Tree: all levels filled except last (left filled first)
                      •	Height = max depth from root to leaf
                      •	Traversal methods are key
                      Simple Example (Node structure in JavaScript):
                      class Node {
                      constructor(value) {
                        this.value = value;
                        this.left = null;
                        this.right = null;
                      }
                      }
                      ________________________________________
                      📘 35. Binary Search Tree (BST)
                      Description:
                      A BST is a binary tree where the left child has smaller value and the right child has larger value than the parent node.
                      Main Points:
                      •	Enables efficient search, insert, and delete (O(log n) average)
                      •	Inorder traversal returns sorted data
                      •	Skewed BSTs degrade to linked list (O(n))
                      Simple Example:
                      // Inserting in BST
                      function insert(node, value) {
                      if (!node) return new Node(value);
                      if (value < node.value) node.left = insert(node.left, value);
                      else node.right = insert(node.right, value);
                      return node;
                      }
                      ________________________________________
                      📘 36. AVL Tree
                      Description:
                      An AVL Tree is a self-balancing Binary Search Tree where the difference between the heights of left and right subtrees (balance factor) is at most 1.
                      Main Points:
                      •	Rotations used: Left, Right, Left-Right, Right-Left
                      •	Guarantees O(log n) time for operations
                      •	Used when balanced search performance is needed
                      Simple Example (Balance Factor check):
                      let balanceFactor = height(node.left) - height(node.right);
                      if (balanceFactor > 1 || balanceFactor < -1) {
                      // Tree needs rotation
                      }
                      ________________________________________
                      📘 37. B Tree
                      Description:
                      A B Tree is a self-balancing search tree used primarily in databases and file systems for fast disk access. It can have more than two children.
                      Main Points:
                      •	Generalization of BST; multiple keys per node
                      •	Keeps data sorted and allows binary-like search
                      •	All leaf nodes at the same level
                      •	Minimizes disk reads
                      Simple Example (Concept):
                      B-Tree of order 3: each node can have 2 to 3 children and 1 to 2 keys.
                      ________________________________________
                      📘 38. B+ Tree
                      Description:
                      A B+ Tree is an advanced version of the B Tree where all values are stored in leaf nodes, and internal nodes only store keys for routing.
                      Main Points:
                      •	Better suited for range queries and databases
                      •	Leaf nodes are linked for sequential access
                      •	Internal nodes do not store actual data
                      •	All leaf nodes at same level
                      Simple Example (Concept):
                      Root: [20 | 50]
                      Leaf Nodes (linked): [5, 10], [20, 25], [50, 60]
                      ________________________________________
                      📘 39. Red-Black Tree
                      Description:
                      A Red-Black Tree is a self-balancing BST with extra color properties to ensure balance without needing frequent rebalancing.
                      Main Points:
                      •	Each node is either red or black
                      •	Root and leaves are always black
                      •	Red node cannot have red child (no two reds in a row)
                      •	Every path from root to leaf has same number of black nodes
                      •	Guarantees O(log n) operations
                      Simple Example (Color rules):
                      // Insert logic includes re-coloring and rotating
                      ________________________________________
                      📘 40. AA Tree in Data Structure
                      Description:
                      An AA Tree is a form of balanced binary search tree similar to a red-black tree but easier to implement, using levels instead of colors.
                      Main Points:
                      •	Only right links can increase level
                      •	Simpler balancing logic compared to red-black trees
                      •	Operations: Skew (rotation) and Split (promotion)
                      •	Guarantees O(log n) time complexity
                      Simple Example (Conceptual operation):
                      Skew: right rotation to eliminate left horizontal link  
                      Split: left rotation to eliminate two consecutive right links
                      ________________________________________
                      📘 41. DS Graph
                      Description:
                      A Graph is a non-linear data structure consisting of nodes (vertices) and edges connecting them. It models networks, like social graphs or transportation maps.
                      Main Points:
                      •	Can be directed or undirected
                      •	May be weighted or unweighted
                      •	Used in routing, web crawling, networking, etc.
                      •	Not necessarily hierarchical or ordered
                      Simple Example (Undirected Graph):
                      A —— B
                      |     |
                      C —— D
                      ________________________________________
                      📘 42. Graph (Data Structure)
                      Description:
                      In DS, a Graph is a collection of vertices (V) and edges (E). It represents relationships or connections between pairs of elements.
                      Main Points:
                      •	Edges can represent cost, time, distance, etc.
                      •	Types: Directed, Undirected, Weighted, Unweighted, Cyclic, Acyclic
                      •	Common problems: pathfinding, connectivity, cycle detection
                      Simple Example (Edge List):
                      let graph = [
                      ['A', 'B'],
                      ['A', 'C'],
                      ['B', 'D']
                      ];
                      ________________________________________
                      📘 43. Graph Representation in Data Structure
                      Description:
                      Graphs can be represented in multiple formats depending on space and operation needs.
                      Main Points:
                      •	Adjacency Matrix: 2D array, fast lookup, space heavy (O(V²))
                      •	Adjacency List: Array of lists/maps, space efficient (O(V+E))
                      •	Edge List: Array of edge pairs, simple
                      Simple Example (Adjacency List in JS):
                      let adjList = {
                      A: ['B', 'C'],
                      B: ['A', 'D'],
                      C: ['A'],
                      D: ['B']
                      };
                      ________________________________________
                      📘 44. Breadth First Search (BFS) Algorithm
                      Description:
                      BFS explores all neighbors of a node before moving to the next level — ideal for shortest path in unweighted graphs.
                      Main Points:
                      •	Uses a Queue
                      •	Traverses level by level
                      •	Time complexity: O(V + E)
                      •	Good for shortest path, finding connected components
                      Simple Example:
                      function bfs(graph, start) {
                      let visited = new Set();
                      let queue = [start];
                      while (queue.length) {
                        let node = queue.shift();
                        if (!visited.has(node)) {
                          visited.add(node);
                          queue.push(...graph[node]);
                        }
                      }
                      }
                      ________________________________________
                      📘 45. Depth First Search (DFS) Algorithm
                      Description:
                      DFS explores as far down one branch as possible before backtracking — ideal for cycle detection, topological sort, and connected components.
                      Main Points:
                      •	Uses Stack (recursion or explicit)
                      •	Explores deep before wide
                      •	Time complexity: O(V + E)
                      •	Can be recursive or iterative
                      Simple Example:
                      function dfs(graph, node, visited = new Set()) {
                      if (visited.has(node)) return;
                      visited.add(node);
                      for (let neighbor of graph[node]) {
                        dfs(graph, neighbor, visited);
                      }
                      }
                      ________________________________________
                      📘 46. Minimum Spanning Tree (MST)
                      Description:
                      An MST is a subset of edges that connects all vertices in a weighted graph with minimum total edge weight and no cycles.
                      Main Points:
                      •	Only for connected, undirected, weighted graphs
                      •	Total weight is minimized
                      •	Used in network design, circuit layout
                      •	Algorithms: Prim’s, Kruskal’s
                      Simple Concept:
                      •	Given a graph with 5 cities and distances, MST connects all cities with shortest possible roads.
                      ________________________________________
                      📘 47. Prim’s Algorithm
                      Description:
                      Prim’s Algorithm builds the MST by starting from one node and adding the lowest weight edge that connects to the growing tree.
                      Main Points:
                      •	Greedy algorithm
                      •	Uses a priority queue or min-heap
                      •	Time complexity: O(E log V) with heap
                      •	Better for dense graphs
                      Simple Idea:
                      •	Start from any vertex
                      •	Always pick the cheapest edge to a new node
                      ________________________________________
                      📘 48. Kruskal’s Algorithm
                      Description:
                      Kruskal’s Algorithm creates MST by sorting all edges and adding the smallest edge that doesn’t form a cycle.
                      Main Points:
                      •	Greedy algorithm
                      •	Uses Union-Find to detect cycles
                      •	Time complexity: O(E log E)
                      •	Works better for sparse graphs
                      Simple Steps:
                      1.	Sort edges by weight
                      2.	Add edge if it doesn’t form a cycle
                      3.	Stop when V-1 edges added
                      ________________________________________
                      📘 49. Types of Graph in Data Structure
                      Description:
                      Graphs can be classified based on direction, weight, connectivity, and cycles.
                      Main Points:
                      •	Directed vs Undirected
                      •	Weighted vs Unweighted
                      •	Cyclic vs Acyclic
                      •	Connected vs Disconnected
                      •	Dense vs Sparse
                      Simple Table:
                      Type	Example Use
                      Directed	Web links (A → B)
                      Undirected	Friendships (A — B)
                      Weighted	Road map with distances
                      Acyclic	Task dependencies (DAG)
                      ________________________________________
                      📘 50. DS Searching
                      Description:
                      Searching is the process of finding a specific element in a data structure like an array or list.
                      Main Points:
                      •	Two main types: Linear Search and Binary Search
                      •	Efficiency depends on the structure and whether it’s sorted
                      •	Binary Search is faster but requires sorted data
                      Simple Example:
                      // Searching for 5 in [1, 2, 3, 5]
                      let arr = [1, 2, 3, 5];
                      console.log(arr.includes(5)); // true
                      ________________________________________
                      📘 51. Linear Search
                      Description:
                      Linear Search checks each element one-by-one until the target is found or the end is reached.
                      Main Points:
                      •	Simple to implement
                      •	Works on unsorted data
                      •	Time Complexity: O(n)
                      Simple Example:
                      function linearSearch(arr, target) {
                      for (let i = 0; i < arr.length; i++) {
                        if (arr[i] === target) return i;
                      }
                      return -1;
                      }
                      ________________________________________
                      📘 52. Binary Search
                      Description:
                      Binary Search works by repeatedly dividing a sorted array in half to find the target.
                      Main Points:
                      •	Requires sorted array
                      •	Very efficient: Time Complexity: O(log n)
                      •	Divide-and-conquer strategy
                      Simple Example:
                      function binarySearch(arr, target) {
                      let left = 0, right = arr.length - 1;
                      while (left <= right) {
                        let mid = Math.floor((left + right) / 2);
                        if (arr[mid] === target) return mid;
                        else if (arr[mid] < target) left = mid + 1;
                        else right = mid - 1;
                      }
                      return -1;
                      }
                      ________________________________________
                      📘 53. DS Sorting
                      Description:
                      Sorting means arranging elements in a particular order (ascending or descending) to improve search efficiency and readability.
                      Main Points:
                      •	Improves performance for searching and algorithms
                      •	Many sorting algorithms vary by time/space complexity
                      •	Categories: Comparison-based, Non-comparison-based
                      Simple Example:
                      let nums = [3, 1, 4];
                      nums.sort(); // Output: [1, 3, 4]
                      ________________________________________
                      📘 54. Sorting Algorithms
                      Description:
                      Sorting algorithms are methods for ordering elements. They differ in performance, stability, and use case.
                      Main Points:
                      •	Stable sort maintains relative order of equal elements
                      •	Choose based on data size, memory, and performance needs
                      •	Types: Bubble, Selection, Insertion, Merge, Quick, Heap, etc.
                      ________________________________________
                      📘 55. Bubble Sort Algorithm
                      Description:
                      Bubble Sort compares and swaps adjacent elements repeatedly until the array is sorted.
                      Main Points:
                      •	Easy to understand
                      •	Stable sorting
                      •	Time: O(n²)
                      Simple Example:
                      function bubbleSort(arr) {
                      for (let i = 0; i < arr.length - 1; i++) {
                        for (let j = 0; j < arr.length - i - 1; j++) {
                          if (arr[j] > arr[j + 1]) [arr[j], arr[j + 1]] = [arr[j + 1], arr[j]];
                        }
                      }
                      }
                      ________________________________________
                      📘 56. Insertion Sort Algorithm
                      Description:
                      Insertion Sort builds the sorted array one element at a time by inserting elements at their correct position.
                      Main Points:
                      •	Simple and good for small datasets
                      •	Stable
                      •	Time: O(n²) average/worst
                      Simple Example:
                      function insertionSort(arr) {
                      for (let i = 1; i < arr.length; i++) {
                        let key = arr[i], j = i - 1;
                        while (j >= 0 && arr[j] > key) {
                          arr[j + 1] = arr[j];
                          j--;
                        }
                        arr[j + 1] = key;
                      }
                      }
                      ________________________________________
                      📘 57. Selection Sort Algorithm
                      Description:
                      Selection Sort selects the smallest element in each pass and moves it to the beginning.
                      Main Points:
                      •	Not stable
                      •	Simple logic but inefficient
                      •	Time: O(n²)
                      Simple Example:
                      function selectionSort(arr) {
                      for (let i = 0; i < arr.length; i++) {
                        let min = i;
                        for (let j = i + 1; j < arr.length; j++) {
                          if (arr[j] < arr[min]) min = j;
                        }
                        [arr[i], arr[min]] = [arr[min], arr[i]];
                      }
                      }
                      ________________________________________
                      📘 58. Quick Sort Algorithm
                      Description:
                      Quick Sort is a divide-and-conquer algorithm that picks a pivot, partitions the array, and recursively sorts the subarrays.
                      Main Points:
                      •	Very fast on average
                      •	Not stable
                      •	Time: O(n log n) average, O(n²) worst
                      Simple Example:
                      function quickSort(arr) {
                      if (arr.length <= 1) return arr;
                      let pivot = arr[arr.length - 1];
                      let left = arr.filter(x => x < pivot);
                      let right = arr.filter(x => x > pivot);
                      let middle = arr.filter(x => x === pivot);
                      return [...quickSort(left), ...middle, ...quickSort(right)];
                      }
                      ________________________________________
                      📘 59. Merge Sort Algorithm
                      Description:
                      Merge Sort divides the array into halves, sorts them, and merges the sorted halves.
                      Main Points:
                      •	Stable
                      •	Good for large datasets
                      •	Time: O(n log n)
                      Simple Example:
                      function mergeSort(arr) {
                      if (arr.length <= 1) return arr;
                      let mid = Math.floor(arr.length / 2);
                      let left = mergeSort(arr.slice(0, mid));
                      let right = mergeSort(arr.slice(mid));
                      return merge(left, right);
                      }
                      
                      function merge(a, b) {
                      let result = [], i = 0, j = 0;
                      while (i < a.length && j < b.length) {
                        result.push(a[i] < b[j] ? a[i++] : b[j++]);
                      }
                      return result.concat(a.slice(i)).concat(b.slice(j));
                      }
                      ________________________________________
                      📘 60. Heap Sort Algorithm
                      Description:
                      Heap Sort uses a binary heap to repeatedly extract the maximum (or minimum) element.
                      Main Points:
                      •	Not stable
                      •	In-place, good time complexity
                      •	Time: O(n log n)
                      Simple Concept:
                      •	Build max-heap → repeatedly remove root → heapify
                      ________________________________________
                      📘 61. Radix Sort Algorithm
                      Description:
                      Radix Sort sorts numbers by processing each digit from least significant to most significant.
                      Main Points:
                      •	Non-comparison based
                      •	Works only on integers (or strings with fixed length)
                      •	Time: O(nk), where k = number of digits
                      Simple Concept:
                      •	Sort by 1s digit, then 10s, then 100s...
                      ________________________________________
                      📘 62. Counting Sort Algorithm
                      Description:
                      Counting Sort counts the occurrences of each value, then calculates positions.
                      Main Points:
                      •	Only for integers in known range
                      •	Stable and fast
                      •	Time: O(n + k), where k = max value
                      Simple Concept:
                      •	Count frequencies → compute positions → fill output array
                      ________________________________________
                      📘 63. Shell Sort Algorithm
                      Description:
                      Shell Sort is a variation of insertion sort that allows comparison and exchange of far-apart elements.
                      Main Points:
                      •	Uses gaps that reduce over time
                      •	Not stable
                      •	Time: O(n log n) average (depends on gap)
                      ________________________________________
                      📘 64. Bucket Sort Algorithm
                      Description:
                      Bucket Sort divides elements into buckets, sorts each bucket, then merges them.
                      Main Points:
                      •	Best for uniformly distributed data
                      •	Can use any sorting algorithm inside buckets
                      •	Time: O(n + k) average
                      ________________________________________
                      📘 65. Time Complexity of Sorting Algorithms
                      Description:
                      This compares the efficiency of common sorting algorithms in best, average, and worst cases.
                      Main Points:
                      Algorithm	Best	Average	Worst	Stable?
                      Bubble Sort	O(n)	O(n²)	O(n²)	Yes
                      Selection Sort	O(n²)	O(n²)	O(n²)	No
                      Insertion Sort	O(n)	O(n²)	O(n²)	Yes
                      Merge Sort	O(n log n)	O(n log n)	O(n log n)	Yes
                      Quick Sort	O(n log n)	O(n log n)	O(n²)	No
                      Heap Sort	O(n log n)	O(n log n)	O(n log n)	No
                      Counting Sort	O(n + k)	O(n + k)	O(n + k)	Yes
                      Radix Sort	O(nk)	O(nk)	O(nk)	Yes
                      Bucket Sort	O(n + k)	O(n + k)	O(n²)	Yes
                      ________________________________________
                      📘 66. Hashing in Data Structure
                      Description:
                      Hashing is a technique used to map data of arbitrary size to fixed-size values (hash codes) for fast lookup in data structures like hash tables.
                      Main Points:
                      •	Efficient for searching, insertion, and deletion (average O(1))
                      •	Commonly used in dictionaries, caches, and sets
                      •	May lead to collisions when multiple keys map to the same index
                      •	Collisions are handled by chaining or open addressing
                      Simple Example (JavaScript):
                      js
                      CopyEdit
                      let map = {};
                      map["apple"] = 10;
                      console.log(map["apple"]); // 10
                      ________________________________________
                      📘 67. Hash Functions in Data Structure
                      Description:
                      A hash function converts an input (key) into an integer index for placing values in a hash table.
                      Main Points:
                      •	Should distribute keys uniformly
                      •	Must be deterministic (same key → same hash)
                      •	Examples: modulo operation, polynomial rolling hash
                      •	Good hash functions minimize collisions
                      Simple Example:
                      js
                      CopyEdit
                      function simpleHash(key, size) {
                      let hash = 0;
                      for (let i = 0; i < key.length; i++) {
                        hash += key.charCodeAt(i);
                      }
                      return hash % size;
                      }
                      ________________________________________
                      📘 68. Hash Table in Data Structure
                      Description:
                      A Hash Table stores key-value pairs using a hash function to compute an index into an array of buckets.
                      Main Points:
                      •	Average time: O(1) for search, insert, delete
                      •	Handles collisions with chaining (linked list) or open addressing
                      •	Load factor affects performance
                      Simple Example (Chaining):
                      js
                      CopyEdit
                      let hashTable = [
                      [], [], []
                      ];
                      
                      function insert(key, value) {
                      let index = key.length % 3;
                      hashTable[index].push([key, value]);
                      }
                      ________________________________________
                      📘 69. Heap Data Structure
                      Description:
                      A Heap is a complete binary tree where the parent node is either greater (max-heap) or smaller (min-heap) than its children.
                      Main Points:
                      •	Used in priority queues, heap sort, Dijkstra’s algorithm
                      •	Supports insert, delete, and extract operations efficiently
                      •	Min-heap: smallest element at root
                      Max-heap: largest element at root
                      •	Time complexity: O(log n) for insertion and deletion
                      Simple Example (Min Heap Array):
                      [2, 3, 4, 6, 5, 9]
                      ________________________________________
                      📘 70. Binomial Heap
                      Description:
                      A Binomial Heap is a collection of binomial trees that satisfy the heap property, optimized for merge operations.
                      Main Points:
                      •	Combines multiple binomial trees with increasing order
                      •	Efficient merge/join of two heaps in O(log n)
                      •	Used in advanced applications like network optimization
                      Key Operations:
                      •	Insert: O(log n)
                      •	Merge: O(log n)
                      •	Extract min: O(log n)
                      Simple Example:
                      A binomial heap may look like several tree structures of size 1, 2, 4, etc.
                      ________________________________________
                      📘 71. Fibonacci Heap
                      Description:
                      A Fibonacci Heap is a collection of trees that follow the min-heap property, offering better amortized time complexities.
                      Main Points:
                      •	Insert, Decrease key: O(1) amortized
                      •	Extract min: O(log n) amortized
                      •	Excellent for algorithms like Dijkstra and Prim
                      Structure Highlights:
                      •	Lazy merging
                      •	Circular doubly linked list for root list
                      Simple Analogy:
                      Like a dynamic binomial heap but with more relaxed constraints, allowing faster operations over time.
                      ________________________________________
                      📘 72. Differences: Linear vs Non-Linear Data Structure
                      Description:
                      Compares the organization and traversal pattern of linear vs non-linear data structures.
                      Main Points:
                      •	Linear DS: Elements form a sequence (e.g., array, list, stack, queue)
                      •	Non-linear DS: Elements form a hierarchy (e.g., trees, graphs)
                      •	Traversal: Linear = one level; Non-linear = multiple paths
                      •	Memory: Easier in linear; complex in non-linear
                      Example:
                      •	Array (Linear): [10, 20, 30]
                      •	Tree (Non-Linear):
                        10
                       /  \
                      20  30
                      ________________________________________
                      📘 73. Difference between Array and Linked List
                      Main Points:
                      Feature	Array	Linked List
                      Memory	Contiguous	Non-contiguous (dynamic)
                      Insertion	Costly (shifting needed)	Easy (change pointers)
                      Access	O(1) random access	O(n) traversal
                      Size	Fixed	Dynamic
                      Example:
                      •	Array: arr[2]
                      •	Linked List: head -> node1 -> node2
                      ________________________________________
                      📘 74. Difference between Stack and Queue
                      Main Points:
                      Feature	Stack (LIFO)	Queue (FIFO)
                      Access	Top only	Front for removal, rear for insertion
                      Order	Last In First Out	First In First Out
                      Use case	Backtracking, Undo	Scheduling, Print Queue
                      Example:
                      •	Stack: Push(1), Push(2), Pop() => 2
                      •	Queue: Enqueue(1), Enqueue(2), Dequeue() => 1
                      ________________________________________
                      📘 75. Linear Queue vs Circular Queue
                      Main Points:
                      Feature	Linear Queue	Circular Queue
                      Space	Wasted after deletion	Reused
                      Pointer movement	One direction	Wraps around
                      Overflow	Premature	Delayed
                      Example:
                      •	Circular queue reuses array spaces after front moves.
                      ________________________________________
                      📘 76. Linear Search vs Binary Search
                      Main Points:
                      Feature	Linear Search	Binary Search
                      Data Order	Any order	Sorted only
                      Time Complexity	O(n)	O(log n)
                      Technique	Sequential scan	Divide and conquer
                      Example:
                      •	Binary Search: [1, 3, 5, 7] → search 5
                      ________________________________________
                      📘 77. Singly Linked List vs Doubly Linked List
                      Main Points:
                      Feature	Singly Linked List	Doubly Linked List
                      Pointers	One (next)	Two (next, prev)
                      Navigation	One direction	Both directions
                      Memory	Less	More (extra pointer)
                      Example:
                      •	DLL: prev <- node <-> node -> next
                      ________________________________________
                      📘 78. Binary Tree vs Binary Search Tree
                      Main Points:
                      Feature	Binary Tree	Binary Search Tree (BST)
                      Ordering	No specific order	Left < Root < Right
                      Usage	General hierarchy	Efficient search
                      Traversal	Unstructured	In-order = sorted data
                      ________________________________________
                      📘 79. Tree vs Graph
                      Main Points:
                      Feature	Tree	Graph
                      Structure	Hierarchical (acyclic)	Can be cyclic/acyclic
                      Connectivity	One path between nodes	Multiple possible paths
                      Root	Has root	May not have a root
                      ________________________________________
                      📘 80. BST vs AVL Tree
                      Main Points:
                      Feature	Binary Search Tree	AVL Tree
                      Balance	Not self-balancing	Self-balancing
                      Efficiency	May degrade to O(n)	Guarantees O(log n)
                      Rotations	No	Yes
                      ________________________________________
                      📘 81. Red Black Tree vs AVL Tree
                      Main Points:
                      Feature	Red Black Tree	AVL Tree
                      Balance	Less strict	More strict
                      Rotations	Fewer	More
                      Insert/Delete	Faster	Slower but more balanced
                      ________________________________________
                      📘 82. B Tree vs B+ Tree
                      Main Points:
                      Feature	B Tree	B+ Tree
                      Data in leaf	Internal + leaves	Leaves only
                      Search	Slower	Faster (linked leaves)
                      Range query	Less efficient	Very efficient
                      ________________________________________
                      📘 83. Quick Sort vs Merge Sort
                      Main Points:
                      Feature	Quick Sort	Merge Sort
                      Type	In-place	Not in-place (extra space)
                      Speed	Faster on average	More predictable
                      Worst Case	O(n²)	O(n log n)
                      ________________________________________
                      📘 84. BFS vs DFS
                      Main Points:
                      Feature	BFS	DFS
                      Structure	Queue	Stack/Recursion
                      Traversal	Level-order	Depth-first
                      Memory	More	Less
                      ________________________________________
                      📘 85. Stack vs Heap
                      Main Points:
                      Feature	Stack (Memory)	Heap (Memory)
                      Allocation	Static	Dynamic
                      Speed	Faster	Slower
                      Size limit	Small	Large
                      ________________________________________
                      📘 86. Bubble Sort vs Selection Sort
                      Main Points:
                      Feature	Bubble Sort	Selection Sort
                      Technique	Swaps adjacent elements	Selects min & swaps
                      Passes	More	Fewer
                      Best use	Nearly sorted	Small lists
                      ________________________________________
                      📘 87. Stack vs Array
                      Main Points:
                      Feature	Stack	Array
                      Access	Only top	Random access
                      Operations	push, pop	Any index
                      Usage	LIFO operations	General data storage
                      ________________________________________
                      📘 88. Full Binary Tree vs Complete Binary Tree
                      Main Points:
                      Feature	Full Binary Tree	Complete Binary Tree
                      Node Degree	0 or 2	All levels full except last
                      Shape	Symmetrical	Left aligned
                      ________________________________________
                      📘 89. B-Tree vs Binary Tree
                      Main Points:
                      Feature	B-Tree	Binary Tree
                      Children	Many	2 at most
                      Height	Shorter (multi-way)	Taller
                      Usage	Databases, Filesystems	General structure
                      ________________________________________
                      📘 90. Primitive vs Non-Primitive Data Structures
                      Main Points:
                      Feature	Primitive	Non-Primitive
                      Examples	int, char, float	Arrays, Lists, Trees
                      Built-in	Yes	User-defined
                      ________________________________________
                      📘 91. Data Type vs Data Structure
                      Main Points:
                      Feature	Data Type	Data Structure
                      Purpose	Represents type of data	Organizes data
                      Examples	int, float, char	stack, queue, graph
                      ________________________________________
                      📘 92. Array-Based Queue vs List-Based Queue
                      Main Points:
                      Feature	Array Queue	Linked List Queue
                      Size	Fixed	Dynamic
                      Memory usage	Wasted in resizing	Efficient
                      Implementation	Easier	Slightly complex
                      
                      •	Binary Search Tree (BST)
                      •	Searching, Insertion, Deletion in BST
                      ________________________________________
                      📘 93. List-Based Queues
                      Description:
                      A List-Based Queue is a dynamic queue implemented using a linked list structure, which grows as needed.
                      Main Points:
                      •	No size limit like arrays.
                      •	Enqueue at tail, dequeue from head.
                      •	Efficient O(1) insertion/deletion (with tail pointer).
                      Example Logic (Linked List Queue):
                      class Node {
                      constructor(data) {
                        this.data = data;
                        this.next = null;
                      }
                      }
                      
                      class Queue {
                      constructor() {
                        this.front = this.rear = null;
                      }
                      
                      enqueue(data) {
                        let newNode = new Node(data);
                        if (!this.rear) this.front = this.rear = newNode;
                        else {
                          this.rear.next = newNode;
                          this.rear = newNode;
                        }
                      }
                      
                      dequeue() {
                        if (!this.front) return null;
                        let removed = this.front.data;
                        this.front = this.front.next;
                        if (!this.front) this.rear = null;
                        return removed;
                      }
                      }
                      ________________________________________
                      📘 94. Binary Tree
                      Description:
                      A Binary Tree is a hierarchical data structure where each node has at most two children: left and right.
                      Main Points:
                      •	Root node is the entry point.
                      •	Types: Full, Complete, Perfect, Skewed Trees.
                      •	Used in many hierarchical and structured problems.
                      Example:
                        A
                       / \
                      B   C
                      ________________________________________
                      📘 95. Pre-order Traversal
                      Description:
                      Visits nodes in the order: Root → Left → Right
                      Main Points:
                      •	Root first, then subtrees.
                      •	Used in expression tree evaluations and tree copying.
                      Example Tree:
                      
                      
                        1
                       / \
                      2   3
                      Output: 1 2 3
                      ________________________________________
                      📘 96. In-order Traversal
                      Description:
                      Visits nodes in the order: Left → Root → Right
                      Main Points:
                      •	Gives sorted order in a Binary Search Tree.
                      •	Common in mathematical expression evaluation.
                      Output: 2 1 3
                      ________________________________________
                      📘 97. Post-order Traversal
                      Description:
                      Visits nodes in the order: Left → Right → Root
                      Main Points:
                      •	Used in deletion operations.
                      •	Evaluates expression trees bottom-up.
                      Output: 2 3 1
                      ________________________________________
                      📘 98. Binary Search Tree (BST)
                      Description:
                      A BST is a binary tree where the left child < parent < right child.
                      Main Points:
                      •	Efficient for search, insert, delete operations.
                      •	Balanced BSTs give O(log n) performance.
                      Example:
                      
                      
                        5
                       / \
                      3   8
                      ________________________________________
                      📘 99. Searching in BST
                      Description:
                      Find if a value exists by recursively or iteratively traversing left or right.
                      Main Points:
                      •	If value < node → search left.
                      •	If value > node → search right.
                      •	Stops when value is found or node is null.
                      Example Code:
                      function search(node, key) {
                      if (!node || node.val === key) return node;
                      return key < node.val ? search(node.left, key) : search(node.right, key);
                      }
                      ________________________________________
                      📘 100. Insertion in BST
                      Description:
                      Insert a value while maintaining the BST property.
                      Main Points:
                      •	Recursively find correct position.
                      •	Insert at leaf position.
                      Example Code:
                      function insert(node, key) {
                      if (!node) return new Node(key);
                      if (key < node.val) node.left = insert(node.left, key);
                      else node.right = insert(node.right, key);
                      return node;
                      }
                      ________________________________________
                      📘 101. Deletion in BST
                      Description:
                      Delete a node from a BST while preserving its structure and property.
                      Main Points:
                      •	Case 1: No child → delete node.
                      •	Case 2: One child → replace node with child.
                      •	Case 3: Two children → replace with inorder successor/predecessor.
                      Example Code:
                      js
                      CopyEdit
                      function deleteNode(root, key) {
                      if (!root) return null;
                      if (key < root.val) root.left = deleteNode(root.left, key);
                      else if (key > root.val) root.right = deleteNode(root.right, key);
                      else {
                        if (!root.left) return root.right;
                        if (!root.right) return root.left;
                      
                        let temp = findMin(root.right);
                        root.val = temp.val;
                        root.right = deleteNode(root.right, temp.val);
                      }
                      return root;
                      }
                      function findMin(node) {
                      while (node.left) node = node.left;
                      return node;
                      }
                      
                      Tree operations and various Linked List operations:
                      ________________________________________
                      📘 102. AVL Tree
                      Description:
                      An AVL Tree is a self-balancing Binary Search Tree where the difference between heights of left and right subtrees (balance factor) is at most 1 for every node.
                      Main Points:
                      •	Maintains O(log n) height
                      •	Each rotation (LL, LR, RL, RR) helps maintain balance
                      •	Named after inventors: Adelson-Velsky and Landis
                      Example:
                      Inserting nodes 10, 20, 30 in a BST leads to imbalance. AVL Tree performs LL rotation to balance it.
                      ________________________________________
                      📘 103. Insertion in AVL Tree
                      a) LL Rotation (Left-Left Rotation)
                      Occurs when a node is inserted into the left subtree of the left child.
                      b) LR Rotation (Left-Right Rotation)
                      Occurs when a node is inserted into the right subtree of the left child. Two rotations: left on child, right on root.
                      c) RL Rotation (Right-Left Rotation)
                      Occurs when a node is inserted into the left subtree of the right child. Two rotations: right on child, left on root.
                      d) RR Rotation (Right-Right Rotation)
                      Occurs when a node is inserted into the right subtree of the right child.
                      ________________________________________
                      📘 104. Deletion in AVL Tree
                      Main Points:
                      •	Delete as in normal BST
                      •	Rebalance using rotations during upward traversal
                      •	May trigger LL, RR, LR, or RL rotations
                      Example:
                      Deleting a node may unbalance the tree and a suitable rotation is performed to fix it.
                      ________________________________________
                      📘 105. Singly Linked List – Insertion at Beginning
                      Description:
                      Add a new node at the start. Update head to point to the new node.
                      newNode->next = head;
                      head = newNode;
                      ________________________________________
                      📘 106. Singly Linked List – Insertion at End
                      Description:
                      Traverse to last node, then link last->next = newNode.
                      ________________________________________
                      📘 107. Singly Linked List – Insertion After Specified Node
                      Description:
                      Given a target node, set newNode->next = target->next; target->next = newNode;
                      ________________________________________
                      📘 108. Singly Linked List – Deletion at Beginning
                      Description:
                      Just update head = head->next; and free the old head.
                      ________________________________________
                      📘 109. Singly Linked List – Deletion at End
                      Description:
                      Traverse to second-last node, set its next = NULL, and free last node.
                      ________________________________________
                      📘 110. Singly Linked List – Deletion After Specified Node
                      Description:
                      Update target->next = target->next->next; and delete the node.
                      ________________________________________
                      📘 111. Singly Linked List – Traversing
                      Description:
                      Use loop to visit each node: while(ptr != NULL) { /* do something */ }
                      ________________________________________
                      📘 112. Singly Linked List – Searching
                      Description:
                      Check if (ptr->data == key) while traversing.
                      ________________________________________
                      📘 113. Doubly Linked List – Insertion at Beginning
                      Description:
                      Set newNode->next = head; head->prev = newNode; head = newNode;
                      ________________________________________
                      📘 114. Doubly Linked List – Insertion at End
                      Description:
                      Traverse to end. Set last->next = newNode; newNode->prev = last;
                      ________________________________________
                      📘 115. Doubly Linked List – Insertion After Specified Node
                      Description:
                      Adjust both next and prev pointers of adjacent nodes and new node.
                      ________________________________________
                      📘 116. Doubly Linked List – Deletion at Beginning
                      Description:
                      Update head = head->next; head->prev = NULL; and delete old head.
                      ________________________________________
                      📘 117. Doubly Linked List – Deletion at End
                      Description:
                      Update second-last’s next = NULL; and delete last.
                      ________________________________________
                      📘 118. Doubly Linked List – Deletion of Node Having Given Data
                      Description:
                      Traverse, then use:
                      temp->prev->next = temp->next;
                      temp->next->prev = temp->prev;
                      ________________________________________
                      📘 119. Doubly Linked List – Traversing
                      Description:
                      Can go forward and backward using next and prev respectively.
                      ________________________________________
                      📘 120. Doubly Linked List – Searching
                      Description:
                      Linear search, but can search from either direction.
 </pre>
