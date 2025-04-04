![Image](https://github.com/user-attachments/assets/6264ed6d-d26b-4916-9e28-efff8fe4fa7e)

# DSA Cheatsheet in JavaScript

Welcome to the **DSA Cheatsheet in JavaScript**! 🚀
This repository is a comprehensive guide covering Data Structures and Algorithms (DSA) using JavaScript. The goal is to provide quick reference notes, explanations, and implementations to help developers master DSA concepts effectively.

## 📌 Table of Contents

- [Introduction](#introduction)
- [Complexity Analysis](#complexity-analysis)
- [Data Structures](#data-structures)
  - [Arrays](#arrays)
  - [Linked List](#linked-list)
  - [Stacks](#stacks)
  - [Queues](#queues)
  - [Hash Tables](#hash-tables)
  - [Trees](#trees)
  - [Graphs](#graphs)
- [Algorithms](#algorithms)
  - [Sorting Algorithms](#sorting-algorithms)
  - [Searching Algorithms](#searching-algorithms)
  - [Recursion](#recursion)
  - [Dynamic Programming](#dynamic-programming)
  - [Greedy Algorithms](#greedy-algorithms)
  - [Graph Algorithms](#graph-algorithms)
- [Interview Questions](#interview-questions)
- [Resources](#resources)
- [Contributing](#contributing)
- [License](#license)

---

## 📖 Introduction
This cheatsheet is designed to provide quick reference notes for JavaScript developers who want to strengthen their DSA skills. Each section includes concise explanations, time and space complexity analysis, and JavaScript implementations.

## ⏳ Complexity Analysis
Understanding **Time Complexity** and **Space Complexity** is crucial when analyzing the efficiency of an algorithm.

| Notation | Name          | Description |
|----------|--------------|-------------|
| O(1)     | Constant     | Fastest, doesn't depend on input size |
| O(log n) | Logarithmic  | Efficient, often found in search operations |
| O(n)     | Linear       | Grows proportionally with input size |
| O(n log n) | Linearithmic | Common in efficient sorting algorithms |
| O(n²)    | Quadratic    | Nested loops, can be slow for large inputs |
| O(2ⁿ)    | Exponential  | Extremely slow, often seen in brute force solutions |

## 🏗️ Data Structures

### Arrays
- Access: O(1)
- Search: O(n)
- Insert/Delete: O(n)
```js
const arr = [1, 2, 3, 4, 5];
arr.push(6); // O(1)
arr.pop();   // O(1)
arr.splice(2, 1); // O(n)
```

### Linked List
- Insert/Delete: O(1) (at head)
- Search: O(n)
```js
class Node {
  constructor(value) {
    this.value = value;
    this.next = null;
  }
}
class LinkedList {
  constructor() {
    this.head = null;
  }
  add(value) {
    const newNode = new Node(value);
    newNode.next = this.head;
    this.head = newNode;
  }
}
```

### (More Data Structures Coming Soon...)

## 🔍 Algorithms

### Sorting Algorithms
- Bubble Sort, Selection Sort, Merge Sort, Quick Sort, etc.

### Searching Algorithms
- Linear Search, Binary Search, etc.

### (More Algorithms Coming Soon...)

## ❓ Interview Questions
A collection of frequently asked DSA interview questions and solutions.

## 📚 Resources
- [MDN JavaScript Docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
- [GeeksforGeeks](https://www.geeksforgeeks.org/)
- [LeetCode](https://leetcode.com/)

## 🤝 Contributing
Feel free to contribute to this repository by adding new concepts, explanations, or code implementations.

## 📝 License
This project is licensed under the MIT License.

---

🚀 **Stay tuned! More content will be added gradually.**
