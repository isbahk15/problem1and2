This project contains solutions for two algorithm problems using arrays and nested loops:

Sum of Distinct Elements

Given two arrays (sets), the algorithm calculates the sum of all elements that are present in only one of the sets.

Uses nested loops to compare elements between the arrays.

Demonstrates array manipulation and conditional logic.

Check Orthogonal Vectors (Dot Product)

Computes the dot (scalar) product of two vectors.

Determines whether pairs of vectors are orthogonal (perpendicular) by checking if their dot product is zero.

Demonstrates array usage, nested loops, and procedure calls.

Algorithms Included

SumDistinctElements(Set1[], n, Set2[], m)

Loops through each element of both sets.

Uses a flag (isDistinct) to identify elements unique to one set.

Calculates the sum of all distinct elements.

dot_product(v1[], v2[], n, output ps)

Calculates the dot product of two vectors.

Outer loop iterates over vector elements.

(Optional inner loop included to satisfy nested loop requirement.)

CheckOrthogonalVectors(Pairs, n)

Loops through an array of vector pairs.

Calls dot_product for each pair.

Prints whether vectors are orthogonal or not.