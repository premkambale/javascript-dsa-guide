## Big-O Notation

### What does better code mean?
1. Faster
2. Less memory intensive
3. More Readable

---

### What is Big-O Notation?
Big-O Notation is the mathematical concept used in computer science to describe the **efficiency or performance of an algorithm**.

### Why Use Big-O Notation?
- To compare different algorithms based on their efficiency.
- To understand how an algorithm performs as input size increases.
- Helps in selecting the best approach for a problem.

We say that an algorithm is **O(f(n))**, if the number of simple operations is less than a constant times **f(n)** as **n** increases.

---

### Common Big-O Complexities (From Best to Worst)

| Big-O Notation | Name                 | Performance (as *n* grows) |
|---------------|---------------------|---------------------------|
| **O(1)**      | Constant Time       | Fastest (doesn’t depend on *n*) |
| **O(log n)**  | Logarithmic Time    | Very efficient |
| **O(n)**      | Linear Time         | Grows proportionally with input |
| **O(n log n)**| Linearithmic Time   | Common in sorting algorithms |
| **O(n²)**     | Quadratic Time      | Slow for large inputs |
| **O(2ⁿ)**     | Exponential Time    | Extremely slow |
| **O(n!)**     | Factorial Time      | Worst complexity |

---

### Big-O Shorthand Rules
1. Arithmetic operators are constant **O(1)**.
2. Variable declaration is constant **O(1)**.
3. Accessing an element or value from an array or object is constant **O(1)**.