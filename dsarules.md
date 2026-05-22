🧠 Core Principles

ALWAYS choose the most efficient approach possible.
ALWAYS consider time and space complexity.
PREFER readability first, optimize only when necessary.
AVOID brute-force if better solutions exist.
BREAK problems into smaller subproblems.


📊 Complexity Rules

ALWAYS analyze:

Time Complexity (Big-O)
Space Complexity



Preferred Complexity Targets

O(1) → Best
O(log n) → Very good
O(n) → Acceptable
O(n log n) → Standard (sorting)
O(n²) → Avoid unless necessary


O(n²) → Strongly avoid




🧱 Data Structure Selection Rules
Arrays / Lists

Use for indexed access
Use when size is fixed or predictable

HashMap / Dictionary

Use for:

Fast lookups (O(1))
Frequency counting
Caching



Stack

Use for:

LIFO operations
Recursion simulation
Expression evaluation



Queue

Use for:

FIFO operations
Breadth-First Search (BFS)



Linked List

Use when:

Frequent insertions/deletions
No need for random access



Set

Use when:

Need uniqueness
Membership checking



Heap / Priority Queue

Use for:

Top K problems
Scheduling
Min/Max retrieval



Tree

Use for hierarchical data
Binary Search Tree for ordered operations

Graph

Use for:

Networks
Relationships
Pathfinding




⚙️ Algorithm Selection Rules
Searching

Use Binary Search ONLY on sorted data.
Otherwise use Linear Search.


Sorting

Use built-in sorting unless custom logic needed.
Prefer:

QuickSort / MergeSort (general)
HeapSort (priority-based)




Recursion vs Iteration

Use recursion for:

Trees
Divide and conquer


Avoid deep recursion (stack overflow risk)


Dynamic Programming (DP)


Use when:

Overlapping subproblems exist
Optimal substructure exists



Always:

Start with recursion
Optimize using memoization/tabulation




Greedy Algorithms

Use when:

Local optimal leads to global optimal




Graph Algorithms

BFS → shortest path (unweighted)
DFS → traversal, cycle detection
Dijkstra → shortest path (weighted)
Union-Find → connected components


🔁 Problem-Solving Strategy
AI MUST follow this order:

Understand the problem clearly
Identify input and output
Consider edge cases
Choose appropriate data structure
Choose optimal algorithm
Write clean and modular code
Analyze complexity
Optimize if needed


⚠️ Edge Case Handling
ALWAYS consider:

Empty input
Null values
Single element
Large inputs
Duplicate values
Negative values (if applicable)


🧪 Code Quality Rules

ALWAYS write clean, readable code
USE meaningful variable names
AVOID deeply nested logic
SPLIT logic into functions where needed
ADD comments for complex logic


🚀 Optimization Rules

AVOID nested loops when possible
USE hashing to reduce complexity
USE two-pointer technique where applicable
USE sliding window for subarray problems
USE prefix sums for range queries


🧩 Common Patterns (VERY IMPORTANT)
AI SHOULD recognize these patterns:

Two Pointer
Sliding Window
Fast & Slow Pointer (cycle detection)
Backtracking
Divide and Conquer
Greedy
Dynamic Programming
Graph Traversal (BFS/DFS)


❌ Anti-Patterns (STRICTLY AVOID)

Writing brute-force without considering optimization
Ignoring edge cases
Using wrong data structures
Overcomplicating simple problems
Recomputing values unnecessarily


🔄 Reusability Rules

Reuse logic where possible
Avoid duplicate implementations
Create helper functions


✅ AI Behavior Guidelines

ALWAYS explain chosen approach briefly
ALWAYS include complexity analysis
NEVER return inefficient solutions without reason
ALWAYS prefer optimal data structures
ALWAYS validate input before processing
