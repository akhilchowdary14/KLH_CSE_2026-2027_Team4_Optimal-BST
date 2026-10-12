# Optimal Binary Search Tree Using Dynamic Programming

## Team Members

- Akhil chowdary
- S. Sri Sai Pradyumn

## Project Details

- **Project Title:** Optimal Binary Search Tree Using Dynamic Programming
- **Team:** Team 4
- **Section:** Section 2, Batch A
- **Department:** Computer Science and Engineering (CSE)
- **Supervisor:** Supervisor Name

## 1. Abstract

An Optimal Binary Search Tree (OBST) is a binary search tree designed to minimize the expected search cost for a given set of keys and their search frequencies. A normal Binary Search Tree may not always provide the minimum search cost. This project implements the Optimal Binary Search Tree algorithm using Dynamic Programming to find the most efficient arrangement of keys. The application accepts keys and their frequencies, calculates the optimal tree structure, and displays the minimum weighted search cost. A web-based interface allows users to enter inputs and understand the results visually. This project demonstrates the practical application of Dynamic Programming in solving optimization problems.

## 2. Problem Statement

Construct a Binary Search Tree from sorted keys and their search frequencies such that the total weighted search cost is minimized. The objective is to determine the optimal root and tree structure using Dynamic Programming.

## 3. Objectives

- To understand the concept of an Optimal Binary Search Tree.
- To implement Dynamic Programming for tree optimization.
- To minimize the total weighted search cost.
- To display the optimal tree structure and its calculated cost.
- To provide a simple and interactive web interface.

## 4. Technologies Used

- **Frontend:** HTML, CSS, JavaScript
- **Algorithm:** Dynamic Programming
- **Development Environment:** Visual Studio Code
- **Application Type:** Web Application

## 5. Algorithm

1. Accept sorted keys and their corresponding search frequencies.
2. Initialize a cost table to store minimum search costs.
3. Consider each key as a possible root for every range of keys.
4. Calculate the cost of the left and right subtrees.
5. Add the sum of frequencies for the current range.
6. Select the root that produces the minimum cost.
7. Repeat the process for larger ranges using previously computed results.
8. Construct the optimal tree and display the minimum cost.

## 6. Sample Input

| Key | Frequency |
|---|---:|
| A | 4 |
| B | 2 |
| C | 6 |
| D | 3 |

## 7. Expected Output

- **Optimal Root:** C
- **Minimum Weighted Search Cost:** 26
- **Average Search Cost:** Approximately 1.73

*Note: The sample results assume the standard successful-search OBST cost model, where the root is at level 1 and the cost is the sum of frequency multiplied by search level.*

## 8. Advantages

- Reduces the expected search cost for frequently accessed keys.
- Avoids repeated calculations through Dynamic Programming.
- Demonstrates an important optimization technique in Data Structures and Algorithms.
- Provides a visual and user-friendly way to understand the algorithm.

## 9. Applications

- Database indexing and searching.
- Dictionary and symbol-table implementations.
- Search systems with known access frequencies.
- Optimization of frequently accessed data structures.

## 10. Conclusion

The Optimal Binary Search Tree project demonstrates how Dynamic Programming can be used to construct an efficient search tree based on key frequencies. By evaluating possible roots and selecting the minimum-cost arrangement, the algorithm reduces the expected weighted search cost. The web application provides an interactive way to understand the algorithm, its calculations, and its results.

## 11. Future Scope

- Support for larger sets of keys and frequencies.
- Improved visualization of the generated tree.
- Comparison between a normal Binary Search Tree and an Optimal Binary Search Tree.
- Performance analysis for different input datasets.
- Addition of unsuccessful-search probabilities.

## 12. References

1. Thomas H. Cormen et al., *Introduction to Algorithms*, MIT Press.
2. GeeksforGeeks — [Optimal Binary Search Tree](https://www.geeksforgeeks.org/dsa/optimal-binary-search-tree-dp-24/)
3. Wikipedia — [Optimal Binary Search Tree](https://en.wikipedia.org/wiki/Optimal_binary_search_tree)
4. Programiz — [Dynamic Programming](https://www.programiz.com/dsa/dynamic-programming)

---

**Project:** Optimal Binary Search Tree Using Dynamic Programming  
**Team:** Team 4 | **Section:** Section 2, Batch A | **Department:** CSE

