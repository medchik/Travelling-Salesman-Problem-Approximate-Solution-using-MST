# Travelling-Salesman-Problem-Approximate-Solution-using-MST
Travelling Salesman Problem | Approximate using MST
i have done the implementation of GeeksforGeeks idea , by using MST to find an approximate solution to TSP using JavaScript.
# introduction
We introduced Travelling Salesman Problem and discussed Naive and Dynamic Programming Solutions for the problem in the previous post,. Both of the solutions are infeasible. In fact, there is no polynomial time solution available for this problem as the problem is a known NP-Hard problem. There are approximate algorithms to solve the problem though. The approximate algorithms work only if the problem instance satisfies Triangle-Inequality.

# Triangle-Inequality: 
The least distant path to reach a vertex j from i is always to reach j directly from i, rather than through some other vertex k (or vertices), i.e., dis(i, j) is always less than or equal to dis(i, k) + dist(k, j). The Triangle-Inequality holds in many practical situations.
When the cost function satisfies the triangle inequality, we can design an approximate algorithm for TSP that returns a tour whose cost is never more than twice the cost of an optimal tour. The idea is to use Minimum Spanning Tree (MST). Following is the MST based algorithm
# Algorithm:
1) Let 1 be the starting and ending point for salesman.
2) Construct MST from with 1 as root using Prim’s Algorithm.
3) List vertices visited in preorder walk of the constructed MST and add 1 at the end.

