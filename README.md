# University Project(one year)

Title: Early detection of abnormal conditions of wind turbines

Dataset：Wind turbine prediction competition information provided by Portugal’s EDP Renováveis

change point detection methods in SCADA data with 55 features:

1.Pruned Exact Linear Time (PELT):
- An exact method, typically produces fast and consistent results. It detects change points by minimizing a cost function.
    - Complexity: O(n), where n is the number of data points.

2.Dynamic Programming:
- An exact method
    - Complexity: O(Qn^2), where Q is the maximum number of change points, and n is the number of data points.

3.Binary Segmentation:
- An approximate method, widely used. The algorithm iteratively applies a single change point method to the entire sequence to determine the presence of a split. If a split is detected, the sequence is divided into two subsequences, and the same process is applied to each.
    - Complexity: O(n log n), where n is the number of data points.

4.Window-based:
- A simpler approximate search method. It suggests the presence of a change point where a significant difference between two values appears. After generating a difference curve, the algorithm locates the optimal change point index in the sequence.
