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
[DS1.1] - [Array](https://en.wikipedia.org/wiki/Array_(data_structure))
   - [Dynamic Array](https://en.wikipedia.org/wiki/Dynamic_array)
   - [Circular Array](https://en.wikipedia.org/wiki/Circular_buffer)
   - Time Complexity: Access O(1), Insert/Delete O(n)

[DS1.2] - [Associative Array](https://en.wikipedia.org/wiki/Associative_array)
   - [Dictionary](https://en.wikipedia.org/wiki/Associative_array#Dictionary)
   - [Symbol Table](https://en.wikipedia.org/wiki/Symbol_table)
   - Time Complexity: Average case O(1) for hash tables

[DS1.3] - [Linked List](https://en.wikipedia.org/wiki/Linked_list)
   - [Singly Linked](https://en.wikipedia.org/wiki/Linked_list#Singly_linked_list)
   - [Doubly Linked](https://en.wikipedia.org/wiki/Doubly_linked_list)
   - [XOR Linked Lists](https://en.wikipedia.org/wiki/XOR_linked_list)
   - Time Complexity: Access O(n), Insert/Delete O(1)

[DS1.4] - [Stack](https://en.wikipedia.org/wiki/Stack_(abstract_data_type))
   - [Call Stack](https://en.wikipedia.org/wiki/Call_stack)
   - [Stack Machine](https://en.wikipedia.org/wiki/Stack_machine)
   - Time Complexity: Push/Pop O(1)

[DS1.5] - [Queue](https://en.wikipedia.org/wiki/Queue_(abstract_data_type))
   - [Priority Queue](https://en.wikipedia.org/wiki/Priority_queue)
   - [Double-ended Queue](https://en.wikipedia.org/wiki/Double-ended_queue)
   - [Circular Queue](https://en.wikipedia.org/wiki/Circular_buffer)
   - Time Complexity: Enqueue/Dequeue O(1)

2. Trees and Graphs
[DS2.1] - [Binary Search Tree](https://en.wikipedia.org/wiki/Binary_search_tree)
   - [AVL Tree](https://en.wikipedia.org/wiki/AVL_tree)
   - [Red-Black Tree](https://en.wikipedia.org/wiki/Red%E2%80%93black_tree)
   - [B-Tree](https://en.wikipedia.org/wiki/B-tree)
   - Time Complexity: Average O(log n) for all operations

[DS2.2] - [Fenwick Tree](https://en.wikipedia.org/wiki/Fenwick_tree)
   - [Binary Indexed Tree](https://en.wikipedia.org/wiki/Fenwick_tree)
   - Applications: Range queries and updates
   - Time Complexity: O(log n) for updates and queries

[DS2.3] - [Graph](https://en.wikipedia.org/wiki/Graph_(abstract_data_type))
   - [Directed Graphs](https://en.wikipedia.org/wiki/Directed_graph)
   - [Undirected Graphs](https://en.wikipedia.org/wiki/Graph_(discrete_mathematics)#Undirected_graph)
   - [Weighted Graphs](https://en.wikipedia.org/wiki/Weighted_graph)
   - Common Algorithms: [Dijkstra](https://en.wikipedia.org/wiki/Dijkstra%27s_algorithm), [A*](https://en.wikipedia.org/wiki/A*_search_algorithm)

[DS2.4] - [Heap](https://en.wikipedia.org/wiki/Heap_(data_structure))
   - [Binary Heap](https://en.wikipedia.org/wiki/Binary_heap)
   - [Fibonacci Heap](https://en.wikipedia.org/wiki/Fibonacci_heap)
   - [Binomial Heap](https://en.wikipedia.org/wiki/Binomial_heap)
   - Time Complexity: Insert O(log n), Get-Min O(1)

[DS2.5] - [Segment Tree](https://en.wikipedia.org/wiki/Segment_tree)
   - [Range Queries](https://en.wikipedia.org/wiki/Range_query_(data_structures))
   - [Lazy Propagation](https://en.wikipedia.org/wiki/Segment_tree#Lazy_propagation)
   - Time Complexity: Build O(n), Query/Update O(log n)

[DS2.6] - [Trie](https://en.wikipedia.org/wiki/Trie)
   - [Radix Tree](https://en.wikipedia.org/wiki/Radix_tree)
   - [Suffix Tree](https://en.wikipedia.org/wiki/Suffix_tree)
   - [Patricia Trie](https://en.wikipedia.org/wiki/Radix_tree)
   - Applications: String matching, IP routing

3. Hash-based Structures
- [Hash Table](https://en.wikipedia.org/wiki/Hash_table)

## Sorting Algorithms

1. Theory and Concepts
[ST1.1] - [Computational Complexity Theory](https://en.wikipedia.org/wiki/Computational_complexity_theory)
   - [Time Complexity](https://en.wikipedia.org/wiki/Time_complexity)
   - [Space Complexity](https://en.wikipedia.org/wiki/Space_complexity)
   - [NP-Completeness](https://en.wikipedia.org/wiki/NP-completeness)

[ST1.2] - [Big O Notation](https://en.wikipedia.org/wiki/Big_O_notation)
   - [Best, Average, Worst Cases](https://en.wikipedia.org/wiki/Best,_worst_and_average_case)
   - [Asymptotic Analysis](https://en.wikipedia.org/wiki/Asymptotic_analysis)
   - Common Complexities: O(1), O(log n), O(n), O(n log n), O(n²)

[ST1.3] - [Total Order](https://en.wikipedia.org/wiki/Total_order)
   - [Partial Order](https://en.wikipedia.org/wiki/Partially_ordered_set)
   - [Lexicographical Order](https://en.wikipedia.org/wiki/Lexicographical_order)
   - Applications in Sorting

[ST1.4] - [Stable Sort](https://en.wikipedia.org/wiki/Sorting_algorithm#Stability)
   - [Stability in Sorting](https://en.wikipedia.org/wiki/Sorting_algorithm#Stability)
   - Examples: Merge Sort (stable), Quicksort (unstable)
   - Importance in Real-world Applications

[ST1.5] - [Comparison Sort](https://en.wikipedia.org/wiki/Comparison_sort)
   - [Lower Bounds](https://en.wikipedia.org/wiki/Comparison_sort#Lower_bounds)
   - [Decision Tree Model](https://en.wikipedia.org/wiki/Decision_tree)
   - Theoretical Minimum: Ω(n log n)

[ST1.6] - [Integer Sorting](https://en.wikipedia.org/wiki/Integer_sorting)
   - [Linear Time Sorting](https://en.wikipedia.org/wiki/Sorting_algorithm#Linear_time)
   - [Radix Sort Analysis](https://en.wikipedia.org/wiki/Radix_sort)
   - [Counting Sort Analysis](https://en.wikipedia.org/wiki/Counting_sort)
   - Better than Comparison Sort: O(n)

2. Exchange Sorts
[ES2.1] - [Bubble Sort](https://en.wikipedia.org/wiki/Bubble_sort)
[ES2.2] - [Cocktail Shaker Sort](https://en.wikipedia.org/wiki/Cocktail_shaker_sort)
[ES2.3] - [Quicksort](https://en.wikipedia.org/wiki/Quicksort)
[ES2.4] - [Comb Sort](https://en.wikipedia.org/wiki/Comb_sort)
[ES2.5] - [Gnome Sort](https://en.wikipedia.org/wiki/Gnome_sort)

3. Selection Sorts
[SS3.1] - [Selection Sort](https://en.wikipedia.org/wiki/Selection_sort)
[SS3.2] - [Heapsort](https://en.wikipedia.org/wiki/Heapsort)
[SS3.3] - [Smoothsort](https://en.wikipedia.org/wiki/Smoothsort)
[SS3.4] - [Tournament Sort](https://en.wikipedia.org/wiki/Tournament_sort)
[SS3.5] - [Cycle Sort](https://en.wikipedia.org/wiki/Cycle_sort)

4. Insertion Sorts
[IS4.1] - [Insertion Sort](https://en.wikipedia.org/wiki/Insertion_sort)
[IS4.2] - [Shell Sort](https://en.wikipedia.org/wiki/Shellsort)
[IS4.3] - [Tree Sort](https://en.wikipedia.org/wiki/Tree_sort)
[IS4.4] - [Library Sort](https://en.wikipedia.org/wiki/Library_sort)
[IS4.5] - [Patience Sorting](https://en.wikipedia.org/wiki/Patience_sorting)

5. Merge Sorts
[MS5.1] - [Merge Sort](https://en.wikipedia.org/wiki/Merge_sort)
[MS5.2] - [Cascade Merge Sort](https://en.wikipedia.org/wiki/Merge_sort#Variants)
[MS5.3] - [Oscillating Merge Sort](https://en.wikipedia.org/wiki/Merge_sort#Variants)

6. Distribution Sorts
[DS6.1] - [Bucket Sort](https://en.wikipedia.org/wiki/Bucket_sort)
[DS6.2] - [Counting Sort](https://en.wikipedia.org/wiki/Counting_sort)
[DS6.3] - [Radix Sort](https://en.wikipedia.org/wiki/Radix_sort)
[DS6.4] - [Pigeonhole Sort](https://en.wikipedia.org/wiki/Pigeonhole_sort)
[DS6.5] - [Flash Sort](https://en.wikipedia.org/wiki/Flashsort)

7. Concurrent and Parallel Sorts
[CS7.1] - [Bitonic Sorter](https://en.wikipedia.org/wiki/Bitonic_sorter)
[CS7.2] - [Batcher Odd-Even Mergesort](https://en.wikipedia.org/wiki/Batcher_odd%E2%80%93even_mergesort)
[CS7.3] - [Samplesort](https://en.wikipedia.org/wiki/Samplesort)

8. Hybrid Sorts
[HS8.1] - [Timsort](https://en.wikipedia.org/wiki/Timsort)
[HS8.2] - [Introsort](https://en.wikipedia.org/wiki/Introsort)
[HS8.3] - [Block Merge Sort](https://en.wikipedia.org/wiki/Block_sort)

9. Specialized Sorts
[PS9.1] - [Topological Sort](https://en.wikipedia.org/wiki/Topological_sorting)
[PS9.2] - [Pancake Sort](https://en.wikipedia.org/wiki/Pancake_sorting)
[PS9.3] - [Spaghetti Sort](https://en.wikipedia.org/wiki/Spaghetti_sort)

10. Impractical/Educational Sorts
[ES10.1] - [Bogosort](https://en.wikipedia.org/wiki/Bogosort)
[ES10.2] - [Slowsort](https://en.wikipedia.org/wiki/Slowsort)
[ES10.3] - [Stooge Sort](https://en.wikipedia.org/wiki/Stooge_sort)

## Related Algorithmic Paradigms
1. Search Algorithms
[AP1.1] - [Binary Search](https://en.wikipedia.org/wiki/Binary_search_algorithm)
[AP1.2] - [Breadth-First Search](https://en.wikipedia.org/wiki/Breadth-first_search)
[AP1.3] - [Depth-First Search](https://en.wikipedia.org/wiki/Depth-first_search)

2. Algorithm Design Paradigms
[AP2.1] - [Divide and Conquer](https://en.wikipedia.org/wiki/Divide-and-conquer_algorithm)
[AP2.2] - [Dynamic Programming](https://en.wikipedia.org/wiki/Dynamic_programming)
[AP2.3] - [Greedy Algorithm](https://en.wikipedia.org/wiki/Greedy_algorithm)
[AP2.4] - [Backtracking](https://en.wikipedia.org/wiki/Backtracking)

3. Advanced Topics
[AP3.1] - [String Searching](https://en.wikipedia.org/wiki/String-searching_algorithm)
[AP3.2] - [Graph Theory](https://en.wikipedia.org/wiki/Graph_theory)
[AP3.3] - [Computational Geometry](https://en.wikipedia.org/wiki/Computational_geometry)
[AP3.4] - [NP-Completeness](https://en.wikipedia.org/wiki/NP-completeness)