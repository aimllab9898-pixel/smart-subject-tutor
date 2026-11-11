
# Subject: Data Structures and Algorithms (B.Tech CSE Core)

## Topic 1: Array vs Linked List
An Array is a linear data structure that stores elements in contiguous memory locations. Each element can be accessed directly using its index in O(1) time because the memory address is calculated using the base address and element size. However, inserting or deleting an element in the middle of an array requires shifting subsequent elements, resulting in O(n) time complexity. Arrays generally have a fixed size in static allocation, while dynamic arrays can resize automatically.

A Linked List is a linear data structure consisting of nodes, where each node contains data and a pointer (reference) to the next node. Unlike arrays, linked list nodes are stored in non-contiguous memory locations. Insertion and deletion at a known node position can be performed in O(1) time by updating pointers, but accessing an element requires sequential traversal, resulting in O(n) time complexity. Common types include Singly Linked Lists, Doubly Linked Lists, and Circular Linked Lists.

## Topic 2: Stack and Queue Data Structures
A Stack is a linear data structure that follows the Last-In, First-Out (LIFO) principle, meaning the most recently inserted element is removed first. It supports two primary operations: Push, which inserts an element at the top, and Pop, which removes the top element. Both operations typically take O(1) time. Stack implementations are commonly used in function call management, recursion, expression evaluation, parentheses matching, and undo operations.

A Queue is a linear data structure that follows the First-In, First-Out (FIFO) principle, meaning the first inserted element is removed first. It supports Enqueue, which inserts an element at the rear, and Dequeue, which removes an element from the front. Both operations can be performed in O(1) time using an efficient implementation. Common variations include Circular Queue, Deque (Double-Ended Queue), and Priority Queue. Queues are widely used in CPU scheduling, breadth-first search (BFS), and task processing systems.

## Topic 3: Searching Algorithms (Linear Search and Binary Search)
Searching algorithms are used to locate a specific element, called a key, within a collection of data.
1. Linear Search: Sequentially checks every element until the target is found or the collection ends. It works on both sorted and unsorted arrays and has a time complexity of O(n) in the average and worst cases. Its best-case complexity is O(1) when the target is the first element.
2. Binary Search: Works only on sorted data structures that support efficient indexed access. It repeatedly divides the search interval into two halves by comparing the target with the middle element. If the target is smaller, it searches the left half; otherwise, it searches the right half. Its time complexity is O(log n), making it significantly faster than linear search for large sorted arrays.
3. Time Complexity: Time complexity describes how the execution time of an algorithm grows as the input size increases. Common complexity classes include O(1), O(log n), O(n), O(n log n), O(n²), and O(2ⁿ).

## Topic 4: Sorting Algorithms (Bubble Sort, Merge Sort, and Quick Sort)
Sorting algorithms arrange elements in a specific order, usually ascending or descending, to simplify searching and data processing.
1. Bubble Sort: Repeatedly compares adjacent elements and swaps them if they are in the wrong order. After each complete pass, the largest unsorted element moves to its correct position. Its average and worst-case time complexity is O(n²), while its best-case complexity is O(n) with an optimized implementation that detects whether any swaps occurred.
2. Merge Sort: Uses the Divide and Conquer technique by recursively dividing an array into two halves, sorting each half, and merging the sorted halves. Its best, average, and worst-case time complexity is O(n log n). It is a stable sorting algorithm but typically requires O(n) auxiliary space for arrays.
3. Quick Sort: Selects an element called a Pivot and partitions the array so that smaller elements appear before the pivot and larger elements appear after it. It recursively sorts the resulting partitions. Its average-case time complexity is O(n log n), while its worst-case complexity is O(n²), usually occurring with highly unbalanced partitions. It is generally efficient in practice and can be implemented in-place.

## Topic 5: Trees and Binary Search Trees (BST)
A Tree is a hierarchical, non-linear data structure consisting of nodes connected through edges. The topmost node is called the Root, nodes without children are called Leaf Nodes, and a node's predecessor is called its Parent. A Binary Tree is a tree in which each node can have at most two children, commonly referred to as the Left Child and Right Child.

A Binary Search Tree (BST) is a binary tree that follows an ordering property: all values in the left subtree of a node are smaller than the node's value, while all values in the right subtree are greater. Searching, insertion, and deletion take O(log n) time on average for a reasonably balanced BST, but can degrade to O(n) in the worst case when the tree becomes skewed. Inorder Traversal of a BST produces elements in sorted order. Common tree traversal techniques include Inorder, Preorder, Postorder, and Level Order Traversal.

## Topic 6: Graphs and Graph Traversal (BFS and DFS)
A Graph is a non-linear data structure consisting of Vertices (Nodes) and Edges that connect pairs of vertices. Graphs can be Directed or Undirected, Weighted or Unweighted, and Cyclic or Acyclic. Graphs are commonly represented using an Adjacency Matrix or an Adjacency List. An Adjacency Matrix uses O(V²) space, while an Adjacency List generally requires O(V + E) space, where V represents vertices and E represents edges.

Graph Traversal algorithms systematically visit vertices to explore graph structures.
1. Breadth-First Search (BFS): Explores vertices level by level, visiting all immediate neighbors before moving to the next level. It uses a Queue and has a time complexity of O(V + E) with an adjacency list. BFS can find the shortest path in an unweighted graph.
2. Depth-First Search (DFS): Explores as far as possible along one branch before backtracking. It uses recursion or an explicit Stack and has a time complexity of O(V + E) with an adjacency list. DFS is useful for cycle detection, connected components, and topological sorting in directed acyclic graphs.

## Topic 7: Recursion and Backtracking
Recursion is a programming technique in which a function calls itself to solve smaller instances of the same problem. Every recursive function must have a Base Case that terminates recursion and a Recursive Case that reduces the problem toward the base case. Recursive calls are stored in the Call Stack, which maintains function parameters, local variables, and return addresses. Incorrect or missing base cases can cause infinite recursion or Stack Overflow.

Backtracking is an algorithmic problem-solving technique that builds solutions incrementally and abandons a partial solution whenever it determines that the solution cannot lead to a valid result. It follows a Choose, Explore, and Unchoose approach. Backtracking is commonly used in N-Queens, Sudoku solving, maze traversal, and generating permutations and combinations. Its time complexity is often exponential because it may explore many possible solution paths.

## Topic 8: Dynamic Programming (DP) and Greedy Algorithms
Dynamic Programming is an optimization technique used to solve problems that exhibit two important properties: Overlapping Subproblems and Optimal Substructure. Instead of repeatedly solving the same subproblems, DP stores their results for future reuse.
1. Memoization: A Top-Down approach in which recursion is combined with caching to store previously computed results.
2. Tabulation: A Bottom-Up approach in which smaller subproblems are solved iteratively and stored in a table until the final answer is obtained.
3. Applications: Fibonacci Sequence, 0/1 Knapsack, Longest Common Subsequence (LCS), Matrix Chain Multiplication, and Coin Change.

A Greedy Algorithm makes the locally optimal choice at each step with the intention of achieving a globally optimal solution. Unlike Dynamic Programming, it generally does not reconsider previous decisions. Greedy algorithms work correctly when the problem satisfies the Greedy Choice Property and Optimal Substructure. Common applications include Activity Selection, Fractional Knapsack, Huffman Coding, and Minimum Spanning Tree algorithms such as Prim's and Kruskal's.
