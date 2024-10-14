The Convex Hull Algorithm is used to find the convex hull of a set of points in computational geometry. The convex hull is the smallest convex set that encloses all the points, forming a convex polygon.
Graham's Scan Algorithm
The Graham's Scan algorithm efficiently computes the convex hull of a set of 2D points through the following steps:

Identify the Starting Point: Locate the point with the smallest y-coordinate, which will be part of the convex hull.

Sort Points: Arrange the remaining points by their polar angle relative to the starting point.

Build the Convex Hull: Iterate through the sorted points and:

Add a point to the hull if it forms a left turn with the last two points in the hull.
Remove the last point if a right turn is formed.
Completion: Continue until all points are processed.

This algorithm operates in 𝑂(𝑛log𝑛) time due to the sorting step and efficiently handles large datasets while ensuring accurate results.

