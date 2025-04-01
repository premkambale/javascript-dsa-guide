## 1️⃣ Big-O Notation

### 1.1 What does better code mean?
1. Faster execution time
2. Less memory usage
3. More readable and maintainable

---

### 1.2 What is Big-O Notation?
Big-O Notation is the mathematical concept used in computer science to describe the **efficiency or performance of an algorithm**.

### 1.3 Why Use Big-O Notation?
1. To compare different algorithms based on efficiency.
2. To understand how an algorithm performs as input size increases.
3. Helps in selecting the best approach for solving problems.

We say that an algorithm is **O(f(n))**, if the number of simple operations is less than a constant times **f(n)** as **n** increases.

---

### 1.4 Common Big-O Complexities (From Best to Worst)

| #  | Big-O Notation | Name                 | Performance (as *n* grows) |
|----|---------------|---------------------|---------------------------|
| 1️⃣  | **O(1)**      | Constant Time       | Fastest (doesn’t depend on *n*) |
| 2️⃣  | **O(log n)**  | Logarithmic Time    | Very efficient |
| 3️⃣  | **O(n)**      | Linear Time         | Grows proportionally with input |
| 4️⃣  | **O(n log n)**| Linearithmic Time   | Common in sorting algorithms |
| 5️⃣  | **O(n²)**     | Quadratic Time      | Slow for large inputs |
| 6️⃣  | **O(2ⁿ)**     | Exponential Time    | Extremely slow |
| 7️⃣  | **O(n!)**     | Factorial Time      | Worst complexity |

---

### 1.5 Big-O Shorthand Rules
1. Arithmetic operations are **O(1)** (constant time).
2. Variable declaration is **O(1)**.
3. Accessing an element from an array or object is **O(1)**.

---

## 2️⃣ Time Complexity

### 2.1 What is Time Complexity?
Time complexity is a measure of how the runtime of an algorithm increases as the size of the input (n) grows.
It helps us analyze the efficiency of an algorithm and predict its performance for large inputs.

---

## 3️⃣ Space Complexity

### 3.1 Formula:
**s(n) = O(f(n))**

### 3.2 What is Space Complexity?
Space complexity is the amount of memory an algorithm needs in terms of input size, i.e., **n**.

- **Boolean, undefined, null, and numbers** take constant space in JavaScript.
- **Strings and arrays** depend on their length.
- **Objects** depend on the number of keys.

### 3.3 Example 1: Constant Space Complexity **O(1)**
```js
const addNums = (arr) => {
  let total = 0;
  for (let i = 0; i < arr.length; i++) {
    total += arr[i];
  }
  return total;
};
console.log(addNums([1, 2])); // Output: 3
```
- The variable `total` has a constant space because numbers take constant space in JavaScript.
- **Space Complexity: O(1) (Constant Space).**

### 3.4 Example 2: Linear Space Complexity **O(n)**
```js
const double = (arr) => {
  let total = [];
  for (let i = 0; i < arr.length; i++) {
    total.push(arr[i] * 2);
  }
  return total;
};
console.log(double([1, 23]));
```
- The variable `total` depends on the length of the parameter `arr`.
- **Space Complexity: O(n) (Space grows as input size grows).**

---

## 4️⃣ Logarithms and Logarithmic Complexity

### 4.1 What is a Logarithm?
Logarithm is the power to which a base should be raised to produce a given number.

### 4.2 What is Logarithmic Complexity?
Logarithmic complexity **O(log n)** means that as the input size **n** increases, the number of steps required to complete the task grows very slowly (logarithmically) instead of linearly.

🔹 **In simple terms:** The algorithm **reduces the problem size by half** in each step, making it much faster than **O(n)**.

### 4.3 Example: **Binary Search** (O(log n))
- If we search for a number in a **sorted array** of **1 million elements**:
  - **Linear search (O(n))** → **1 million steps** 😨
  - **Binary search (O(log n))** → **Only ~20 steps!** 🚀