# Exchange Sorts

## Bubble Sort
[ES2.1] - Implementation and Analysis

### Algorithm Description
- Basic implementation
- Optimized implementation with early exit
- Bidirectional bubble sort (cocktail sort)

### Time Complexity
- Best Case: O(n) when array is already sorted
- Average Case: O(n²)
- Worst Case: O(n²)

### Space Complexity
- O(1) - in-place sorting algorithm

### Key Features
- Stable sort
- In-place algorithm
- Adaptive algorithm
- Online algorithm (can sort as data arrives)

### Implementation Techniques
1. Basic Implementation
2. Early Exit Optimization
3. Cocktail Sort Variation
4. Parallel Implementation

### Best Practices
- Use for small datasets
- Consider as educational example
- Prefer other algorithms for production use

### Real-world Applications
1. Educational purposes
2. Small dataset sorting
3. When simplicity is preferred over efficiency

## Quicksort
[ES2.3] - Implementation and Analysis

### Algorithm Description
- Partition schemes
- Pivot selection strategies
- Recursion optimization

### Time Complexity
- Best Case: O(n log n)
- Average Case: O(n log n)
- Worst Case: O(n²)

### Space Complexity
- O(log n) average case
- O(n) worst case due to recursion

### Key Features
- Unstable sort
- In-place algorithm
- Not adaptive
- Recursive implementation

### Implementation Techniques
1. Different partition schemes
2. Pivot selection strategies
3. Three-way partitioning
4. Hybrid with insertion sort

### Best Practices
- Use median-of-three pivot selection
- Switch to insertion sort for small subarrays
- Consider iteration instead of recursion
- Handle duplicate elements efficiently

### Real-world Applications
1. Standard library sort implementation
2. Large dataset sorting
3. When cache efficiency is important
