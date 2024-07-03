# Second Project: Solving the Travelling Salesman Problem

## Overview

The Travelling Salesman Problem (TSP) is a algorithmic problem in the fields of computer science and operations research. It focuses on optimization, where the goal is to determine the shortest possible route that visits a set of given cities and returns to the origin city.

## Project Made with:
   - [João Rebelo](https://github.com/jrebelo08)
   - [David Ferreira](https://github.com/davidsferreira02)
## Objectives

- Explore different algorithms to solve TSP
- Implement a solution and evaluate its performance
- [**Project Description**](/doc/Project2Description.pdf)

## Key Concepts

### What is TSP?

The Travelling Salesman Problem can be summarized as follows:
- **Input**: A list of cities or Edges containing the information on the source/destination, and the distances between each pair of cities.
 <br>***Note***: There are two types of graphs available for parsing, Toy-Graphs and Extra Fully Connected Graphs, more on this in the Project Description.
- **Output**: The shortest possible route that visits each city exactly once and returns to the starting point.

### Importance of TSP

TSP has applications in various fields such as logistics, planning, and the manufacturing of microchips.

## Algorithms we used to Solve TSP

### Exact Algorithms

1. **BackTracking Approach**:
    - The algorithm operates by recursively exploring
      all possible paths, marking nodes as visited or unvisited as it progresses. 
    - For each path, it calculates the total distance traveled and updates the shortest path found
      whenever a shorter complete tour is identified..
    - Computationally expensive, only feasible for Toy Graphs.

### Heuristic Algorithms

1. **Triangular Approximation Heuristic**:
   - This heuristic involves approximating the solution of a problem by considering triangular inequalities.
2. **NearestNeighbour**:
   - The best balance of performance and efficiency.
   - It starts from an arbitrary node and repeatedly visits the nearest node until all nodes are visited.

3. **K-means Clustering NearestNeighbour**:
   - Combines the clustering algorithm with the NearestNeighbour.
   - The graph nodes are divided into a number of clusters.
   - Then the NN heuristic(2.) is applied to each of the clusters.
   - The results are combined to form a complete tour.

4. **LinKernighan**:
   - This algorithm continues to improve the solution by making local changes until no further improvements can be found.
   - Only feasible in small graphs.


