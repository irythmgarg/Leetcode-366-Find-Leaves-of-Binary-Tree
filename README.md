# Leetcode-366-Find-Leaves-of-Binary-Tree
# 🍃 Find Leaves of Binary Tree (LeetCode #366)

Welcome to the **Find Leaves of Binary Tree** solution! 🚀  
This problem asks you to repeatedly remove all the leaves from a binary tree and return them level-by-level — from leaves to root! 🌳

---

## 💡 Problem Summary

Given the root of a binary tree, **collect all the leaves** and remove them.  
Repeat until the tree is empty.  
Return a list of lists representing the sequence of removed leaves at each iteration.

---

## ✅ Key Concepts Used

- 🧠 **Depth-first Search (DFS)**
- 🌱 **Post-order Traversal**
- 📏 **Calculating Height of Subtrees**
- 📦 **Using Ordered `map` to Organize Nodes by Height**

---

## 🧠 Solution Overview

We define the **height of a node** as:
- `0` if it's `NULL`
- `1 + max(leftHeight, rightHeight)` otherwise

This height represents the "round" in which the node becomes a leaf when leaves are pruned iteratively.

        1
       / \
      2   3
     / \
    4   5


[
  [4, 5, 3],  // first layer of leaves
  [2],        // next layer
  [1]         // root
]


✨ Why It Works
We label each node with a height from the bottom up.

The leaves are collected and grouped by height.

Using a map<int, vector<int>> ensures leaves are naturally ordered by height. 📏

👨‍💻 Author

🧑‍🎓 Ridham Garg

🎓 B.Tech Computer Engineering

🏫 Thapar University, Patiala

🆔 Roll Number: 102203014
