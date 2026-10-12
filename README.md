# Optimal-Binary-Search-Tree-Using-Dynamic-Programming

## Team Members

- Akhil chowdary
- S. Sri Sai Pradyumn

# Optimal Binary Search Tree Using Dynamic Programming

## 3. Supervisor

Supervisor Name

## 4. Abstract

An Optimal Binary Search Tree (OBST) is a binary search tree designed to minimize the total weighted search cost based on the frequencies of keys. Traditional Binary Search Trees do not always provide the minimum search cost because their efficiency depends on the arrangement of keys. This project proposes an Optimal Binary Search Tree using Dynamic Programming to determine the most efficient arrangement of keys. The system accepts sorted keys and their corresponding search frequencies, calculates the minimum weighted search cost, and identifies the optimal root of the tree. A web-based application provides an interactive interface for entering inputs and viewing the resulting tree and calculations. The project demonstrates how Dynamic Programming solves optimization problems by avoiding repeated calculations and storing previously computed results.

## 5. Problem Statement

Searching is an important operation in data structures, and the performance of a Binary Search Tree depends on its structure. When some keys are searched more frequently than others, arranging the tree without considering their frequencies may result in a higher total search cost. Given a sorted set of keys and their corresponding search frequencies, the objective of this project is to construct an Optimal Binary Search Tree that minimizes the weighted search cost. The project uses Dynamic Programming to evaluate possible roots and determine the most efficient tree structure. The resulting application displays the optimal root, tree structure, and minimum search cost.

## 6. Objectives

The main objectives of this project are:

- To understand the concept of an Optimal Binary Search Tree.
- To implement the OBST algorithm using Dynamic Programming.
- To accept sorted keys and their corresponding search frequencies.
- To calculate the minimum weighted search cost.
- To identify the optimal root for the given keys.
- To construct and visualize the resulting optimal tree.
- To avoid repeated calculations by storing intermediate results.
- To provide a simple and interactive web application.
- To demonstrate the practical application of Dynamic Programming in Data Structures and Algorithms.

## 2. Design Methodology & Technical Soundness

The project follows a Dynamic Programming approach to construct an Optimal Binary Search Tree with minimum weighted search cost.

### Methodology

Input Sorted Keys and Frequencies

↓

Validate Input Data

↓

Initialize Dynamic Programming Tables

↓

Calculate Costs for Individual Keys

↓

Evaluate Possible Roots for Key Ranges

↓

Store Minimum Costs and Optimal Roots

↓

Construct the Optimal Binary Search Tree

↓

Display the Tree and Minimum Search Cost

↓

Present Results in the Web Application

### Technical Approach

The system accepts a sorted list of keys and their corresponding search frequencies. Dynamic Programming is used to calculate the minimum cost for different ranges of keys.

For each range, the algorithm considers every key as a possible root. It calculates the costs of the left and right subtrees and adds the total frequency of the current range. The root that produces the minimum cost is selected.

The process continues until the optimal cost and root for the complete set of keys are determined. The stored root information is then used to construct the optimal tree.

### Dynamic Programming Recurrence

Let `cost[i][j]` represent the minimum weighted search cost for keys from index `i` to `j`, and let `freq[k]` represent the frequency of key `k`.

For a range containing one or more keys:

`cost[i][j] = min(cost[i][r-1] + cost[r+1][j] + sum(freq[i...j]))`

where `r` represents each possible root in the range.

The cost of an empty subtree is zero.

### Complexity

- **Time Complexity:** O(n³)
- **Space Complexity:** O(n²)

The standard Dynamic Programming implementation evaluates possible roots for each key range. Its time complexity is O(n³), and the cost and root tables require O(n²) space.

The algorithm is suitable for finding an optimal tree when the search frequencies are known in advance.

## 3. Implementation Progress Against Planned Milestones

| Milestone | Planned Work | Status |
|---|---|---|
| 1 | Topic Selection | Completed |
| 2 | Problem Definition | Completed |
| 3 | Objectives Definition | Completed |
| 4 | Study of Dynamic Programming | Completed |
| 5 | Study of Binary Search Trees | Completed |
| 6 | System Design and Methodology | Completed |
| 7 | Input Validation Module | In Progress |
| 8 | Dynamic Programming Cost Calculation | In Progress |
| 9 | Optimal Root Identification | In Progress |
| 10 | Tree Construction and Visualization | In Progress |
| 11 | Web Application Development | In Progress |
| 12 | Testing and Result Verification | In Progress |
| 13 | Documentation and README | In Progress |
| 14 | Final Demonstration and Presentation | Planned |

**Current Phase:** Implementation, Testing, Tree Visualization, and Documentation.

Update the status according to the actual progress of the team before submission.

## 4. Repository Discipline – Commit History, Structure & Documentation

The project repository follows a structured organization to make the source code easy to understand, maintain, test, and evaluate.

### Repository Structure

```text
Optimal-Binary-Search-Tree/
│
├── README.md
├── index.html
├── style.css
├── script.js
│
├── docs/
│   ├── Abstract.docx
│   ├── Project_Report.docx
│   └── System_Architecture.png
│
├── screenshots/
│   ├── Home_Page.png
│   ├── Input_Keys_Frequencies.png
│   └── Optimal_Tree_Result.png
│
└── PPT/
    └── Optimal_BST_Presentation.pptx
```

*Note: This is a suggested structure for the JavaScript web application. Keep only the folders and files that actually exist in your repository, and adjust filenames as necessary.*

### Suggested Commit History

- Initial project setup
- Added project README
- Added project abstract
- Added problem statement and objectives
- Added system design and methodology
- Implemented input validation
- Implemented Dynamic Programming cost calculation
- Added optimal root identification
- Implemented optimal tree construction
- Added tree visualization
- Improved web application interface
- Added sample test cases
- Verified minimum weighted search cost
- Added project screenshots
- Updated project report and documentation
- Added project presentation
- Final testing and cleanup

## 5. Demonstration, Presentation & Response to Queries

### Demonstration

The project will be demonstrated using a sample set of sorted keys and their search frequencies.

**Input:**

```text
Keys: A, B, C, D
Frequencies: 4, 2, 6, 3
```

The system performs the following operations:

- Accepts the keys and frequencies.
- Validates the input data.
- Calculates the minimum weighted search cost using Dynamic Programming.
- Identifies the optimal root.
- Constructs the optimal tree.
- Displays the calculated results.

**Expected Output:**

```text
Optimal Root: C
Minimum Weighted Search Cost: 26
Average Search Cost: Approximately 1.73
```

The expected results use the standard successful-search cost model, where the root is at level 1 and the average cost is the weighted cost divided by the total frequency.

The web application can display the results using:

- An optimal binary tree visualization.
- A table of keys and frequencies.
- The minimum weighted search cost.
- The selected optimal root.
- A summary of the Dynamic Programming results.

### Possible Viva Questions

**1. What is an Optimal Binary Search Tree?**

An OBST is a binary search tree arranged to minimize the weighted search cost based on the frequencies of its keys.

**2. Why is Dynamic Programming used?**

Dynamic Programming stores the results of smaller subproblems and reuses them to calculate the optimal solution efficiently.

**3. What is the time complexity of the standard OBST algorithm?**

The standard Dynamic Programming algorithm has O(n³) time complexity.

**4. What is the space complexity?**

The cost and root tables require O(n²) space.

**5. What is the purpose of search frequencies?**

Frequencies represent how often keys are searched and help determine the most efficient tree structure.

**6. What is the difference between a normal BST and an OBST?**

A normal BST does not necessarily minimize search cost based on frequencies, whereas an OBST is constructed to minimize the weighted search cost.

## 6. Individual Contribution & Team Coordination

### Member 1 – Algorithm & Core Implementation

**Name:** Akhil chowdary

**Responsibilities:**

- Studied Binary Search Trees and Dynamic Programming.
- Defined the project problem and objectives.
- Designed the algorithm for calculating minimum search cost.
- Worked on Dynamic Programming recurrence relations.
- Implemented or contributed to cost calculation.
- Worked on identifying the optimal root.
- Verified the correctness of algorithm results.
- Contributed to testing and code review.

### Member 2 – Web Application, Visualization & Documentation

**Name:** S. Sri Sai Pradyumn

**Responsibilities:**

- Studied the implementation of the Optimal Binary Search Tree.
- Worked on input handling and validation.
- Developed or contributed to the web application interface.
- Worked on tree construction and visualization.
- Assisted with testing and result verification.
- Prepared project documentation and README.
- Organized the project repository.
- Contributed to the project presentation and demonstration.

### Team Coordination

Both team members contribute to:

- Project discussions.
- Algorithm design.
- Code implementation.
- Testing and debugging.
- Verification of calculated results.
- Web application development.
- Documentation and report preparation.
- Presentation preparation.
- Viva preparation.
- Final project submission.

The team coordinates algorithm development, interface design, testing, and documentation to complete the project

