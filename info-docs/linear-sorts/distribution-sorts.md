# Distribution Sorts

## Counting Sort
[DS6.1] - Implementation and Analysis

### Algorithm Description
- Key-based sorting
- Non-comparative algorithm
- Frequency counting approach

### Time Complexity
- Best Case: O(n + k)
- Average Case: O(n + k)
- Worst Case: O(n + k)
where k is the range of input

### Space Complexity
- O(n + k) for auxiliary arrays

### Key Features
- Stable sort
- Not in-place
- Linear time complexity
- Integer/finite range sorting

### Implementation Techniques
1. Basic counting sort
2. Object sorting with keys
3. Parallel implementation
4. Memory-efficient variations

### Best Practices
- Use when range k is O(n)
- Consider space requirements
- Handle negative numbers properly
- Optimize for cache efficiency

### Real-world Applications
1. Sorting integers with known range
2. Radix sort subroutine
3. Score-based rankings

## Radix Sort
[DS6.3] - Implementation and Analysis

### Algorithm Description
- Digit-by-digit sorting
- Non-comparative algorithm
- Multiple passes approach

### Time Complexity
- Best Case: O(d(n + k))
- Average Case: O(d(n + k))
- Worst Case: O(d(n + k))
where d is number of digits, k is range per digit

### Space Complexity
- O(n + k)

### Key Features
- Stable sort
- Not in-place
- Linear time for fixed-length keys
- Integer/string sorting

### Implementation Techniques
1. LSD (Least Significant Digit)
2. MSD (Most Significant Digit)
3. Binary radix implementation
4. Parallel processing

### Best Practices
- Choose appropriate radix size
- Consider memory usage
- Handle variable-length keys
- Optimize digit extraction

### Real-world Applications
1. Integer sorting
2. String sorting
3. Fixed-length records
4. Network routing tables
