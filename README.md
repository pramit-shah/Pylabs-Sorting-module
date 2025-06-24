# Pylabs-Sorting-module
Pylabs Sorting Module V 0.0.0

-----
## Currently as there are various sorting modules that sort in an forward path, we claim to solve that issue
currently as the sorting methodologies are stagnant and solve one methodologies, this sorting method will only need one download and target industry, and will sort all the sorting foundational issues, improvements, within the repository


### what sorting implementations computers used in fields?

    1. Arrays:

Concept: A collection of elements, each identified by an index or key, stored at contiguous memory locations.

Characteristics:

Fixed-size (in most traditional implementations).

Elements can be accessed directly using their index (O(1) time complexity for access).

Adding or removing elements in the middle can be expensive as it requires shifting other elements.

Examples:

A list of student grades: [85, 92, 78, 95]

A grid for a game board: [[X, O, X], [O, O, X], [X, X, O]]

Use Cases: Storing collections of items where access by index is frequent, implementing lookup tables, image processing.

2. Linked Lists:

Concept: A sequence of nodes, where each node contains data and a reference (or pointer) to the next node in the sequence.

Characteristics:

Dynamic size (can grow or shrink easily).

Elements are not stored contiguously in memory.

Insertion and deletion are efficient (O(1)) if you have a pointer to the node before/after the insertion/deletion point.

Accessing an element requires traversing the list from the beginning (O(n) time complexity for access).

Variations:

Singly Linked List: Nodes point only to the next node.

Doubly Linked List: Nodes point to both the next and previous nodes, allowing for traversal in both directions.

Circular Linked List: The last node points back to the first node, forming a circle.

Use Cases: Implementing stacks and queues, managing dynamic data, representing polynomial equations.

3. Stacks:

Concept: A Linear Data Structure that follows the Last-In, First-Out (LIFO) principle. Think of a stack of plates – you can only take the top one off, and you add new ones to the top.

Operations:

push(): Adds an element to the top of the stack.

pop(): Removes the top element from the stack.

peek() (or top()): Returns the top element without removing it.

isEmpty(): Checks if the stack is empty.

Use Cases: Function call management (call stack), undo/redo functionality, expression evaluation, backtracking algorithms.

4. Queues:

Concept: A Linear Data Structure that follows the First-In, First-Out (FIFO) principle. Think of a line at a supermarket – the first person in line is the first to be served.

Operations:

enqueue(): Adds an element to the rear (back) of the queue.

dequeue(): Removes the front element from the queue.

front() (or peek()): Returns the front element without removing it.

isEmpty(): Checks if the queue is empty.

Use Cases: Task scheduling, breadth-first search (BFS) in graphs, managing shared resources, print spooling.

5. Trees:

Concept: A hierarchical data structure consisting of nodes connected by edges, with a single root node at the top. Each node can have zero or more child nodes.

Characteristics:

Non-linear structure.

Excellent for representing hierarchical relationships.

Variations:

Binary Tree: Each node has at most two children (left and right).

Binary Search Tree (BST): A binary tree where the value of each node is greater than or equal to any value in its left subtree and less than or equal to any value in its right subtree. This allows for efficient searching, insertion, and deletion (on average, O(log n)).

AVL Tree/Red-Black Tree: Self-balancing binary search trees that ensure O(log n) performance for all operations by automatically rebalancing themselves after insertions/deletions.

Heaps: A complete binary tree that satisfies the heap property (either a min-heap where the parent is smaller than children, or a max-heap where the parent is larger). Used for priority queues and heapsort.

Tries (Prefix Trees): Used for efficient retrieval of keys stored in the tree, often used for dictionaries and autocomplete.

Use Cases: File systems, database indexing, routing algorithms, decision trees in machine learning.

6. Graphs:

Concept: A non-linear data structure consisting of a set of vertices (nodes) and a set of edges connecting pairs of vertices.

Characteristics:

Can represent complex relationships between entities.

Edges can be directed (one-way) or undirected (two-way).

Edges can have weights (costs).

Variations:

Directed Graph: Edges have a direction.

Undirected Graph: Edges have no direction.

Weighted Graph: Edges have associated values (weights).

Representations:

Adjacency Matrix: A 2D array where matrix[i][j] indicates if there's an edge between vertex i and vertex j.

Adjacency List: An array of linked lists, where list[i] contains a list of vertices adjacent to vertex i.

Use Cases: Social networks, mapping and navigation systems (shortest path algorithms like Dijkstra's, A*), network topology, dependency resolution.

7. Hash Tables (Hash Maps/Dictionaries/Associative Arrays):

Concept: A data structure that stores key-value pairs, allowing for very fast retrieval of values based on their keys. It uses a hash function to map keys to indices in an array (buckets).

Characteristics:

Provides average O(1) time complexity for insertion, deletion, and retrieval.

Worst-case can be O(n) due to collisions (multiple keys mapping to the same index), which are handled by various collision resolution techniques (e.g., separate chaining, open addressing).

Use Cases: Implementing dictionaries, caches, symbol tables in compilers, database indexing, checking for duplicates.

These are the most fundamental data structures. Many other specialized data structures exist, often built upon these basics, to solve particular problems more efficiently. Understanding these core structures is crucial for anyone working with computer science and programming.

### Sorting Methods known to humankind
--Ref: https://en.wikipedia.org/wiki/Sorting_algorithm

## Data Structures
1. Arrays and Lists
- [Array](https://en.wikipedia.org/wiki/Array_(data_structure))
- [Associative Array](https://en.wikipedia.org/wiki/Associative_array)
- [Linked List](https://en.wikipedia.org/wiki/Linked_list)
- [Stack](https://en.wikipedia.org/wiki/Stack_(abstract_data_type))
- [Queue](https://en.wikipedia.org/wiki/Queue_(abstract_data_type))

2. Trees and Graphs
- [Binary Search Tree](https://en.wikipedia.org/wiki/Binary_search_tree)
- [Fenwick Tree](https://en.wikipedia.org/wiki/Fenwick_tree)
- [Graph](https://en.wikipedia.org/wiki/Graph_(abstract_data_type))
- [Heap](https://en.wikipedia.org/wiki/Heap_(data_structure))
- [Segment Tree](https://en.wikipedia.org/wiki/Segment_tree)
- [Trie](https://en.wikipedia.org/wiki/Trie)

3. Hash-based Structures
- [Hash Table](https://en.wikipedia.org/wiki/Hash_table)

## Sorting Algorithms

1. Theory and Concepts
- [Computational Complexity Theory](https://en.wikipedia.org/wiki/Computational_complexity_theory)
- [Big O Notation](https://en.wikipedia.org/wiki/Big_O_notation)
- [Total Order](https://en.wikipedia.org/wiki/Total_order)
- [Stable Sort](https://en.wikipedia.org/wiki/Sorting_algorithm#Stability)
- [Comparison Sort](https://en.wikipedia.org/wiki/Comparison_sort)
- [Integer Sorting](https://en.wikipedia.org/wiki/Integer_sorting)

2. Exchange Sorts
- [Bubble Sort](https://en.wikipedia.org/wiki/Bubble_sort)
- [Cocktail Shaker Sort](https://en.wikipedia.org/wiki/Cocktail_shaker_sort)
- [Quicksort](https://en.wikipedia.org/wiki/Quicksort)
- [Comb Sort](https://en.wikipedia.org/wiki/Comb_sort)
- [Gnome Sort](https://en.wikipedia.org/wiki/Gnome_sort)

3. Selection Sorts
- [Selection Sort](https://en.wikipedia.org/wiki/Selection_sort)
- [Heapsort](https://en.wikipedia.org/wiki/Heapsort)
- [Smoothsort](https://en.wikipedia.org/wiki/Smoothsort)
- [Tournament Sort](https://en.wikipedia.org/wiki/Tournament_sort)
- [Cycle Sort](https://en.wikipedia.org/wiki/Cycle_sort)

4. Insertion Sorts
- [Insertion Sort](https://en.wikipedia.org/wiki/Insertion_sort)
- [Shell Sort](https://en.wikipedia.org/wiki/Shellsort)
- [Tree Sort](https://en.wikipedia.org/wiki/Tree_sort)
- [Library Sort](https://en.wikipedia.org/wiki/Library_sort)
- [Patience Sorting](https://en.wikipedia.org/wiki/Patience_sorting)

5. Merge Sorts
- [Merge Sort](https://en.wikipedia.org/wiki/Merge_sort)
- [Cascade Merge Sort](https://en.wikipedia.org/wiki/Merge_sort#Variants)
- [Oscillating Merge Sort](https://en.wikipedia.org/wiki/Merge_sort#Variants)

6. Distribution Sorts
- [Bucket Sort](https://en.wikipedia.org/wiki/Bucket_sort)
- [Counting Sort](https://en.wikipedia.org/wiki/Counting_sort)
- [Radix Sort](https://en.wikipedia.org/wiki/Radix_sort)
- [Pigeonhole Sort](https://en.wikipedia.org/wiki/Pigeonhole_sort)
- [Flash Sort](https://en.wikipedia.org/wiki/Flashsort)

7. Concurrent and Parallel Sorts
- [Bitonic Sorter](https://en.wikipedia.org/wiki/Bitonic_sorter)
- [Batcher Odd-Even Mergesort](https://en.wikipedia.org/wiki/Batcher_odd%E2%80%93even_mergesort)
- [Samplesort](https://en.wikipedia.org/wiki/Samplesort)

8. Hybrid Sorts
- [Timsort](https://en.wikipedia.org/wiki/Timsort)
- [Introsort](https://en.wikipedia.org/wiki/Introsort)
- [Block Merge Sort](https://en.wikipedia.org/wiki/Block_sort)

9. Specialized Sorts
- [Topological Sort](https://en.wikipedia.org/wiki/Topological_sorting)
- [Pancake Sort](https://en.wikipedia.org/wiki/Pancake_sorting)
- [Spaghetti Sort](https://en.wikipedia.org/wiki/Spaghetti_sort)

10. Impractical/Educational Sorts
- [Bogosort](https://en.wikipedia.org/wiki/Bogosort)
- [Slowsort](https://en.wikipedia.org/wiki/Slowsort)
- [Stooge Sort](https://en.wikipedia.org/wiki/Stooge_sort)

## Related Algorithmic Paradigms
1. Search Algorithms
- [Binary Search](https://en.wikipedia.org/wiki/Binary_search_algorithm)
- [Breadth-First Search](https://en.wikipedia.org/wiki/Breadth-first_search)
- [Depth-First Search](https://en.wikipedia.org/wiki/Depth-first_search)

2. Algorithm Design Paradigms
- [Divide and Conquer](https://en.wikipedia.org/wiki/Divide-and-conquer_algorithm)
- [Dynamic Programming](https://en.wikipedia.org/wiki/Dynamic_programming)
- [Greedy Algorithm](https://en.wikipedia.org/wiki/Greedy_algorithm)
- [Backtracking](https://en.wikipedia.org/wiki/Backtracking)

3. Advanced Topics
- [String Searching](https://en.wikipedia.org/wiki/String-searching_algorithm)
- [Graph Theory](https://en.wikipedia.org/wiki/Graph_theory)
- [Computational Geometry](https://en.wikipedia.org/wiki/Computational_geometry)
- [NP-Completeness](https://en.wikipedia.org/wiki/NP-completeness)