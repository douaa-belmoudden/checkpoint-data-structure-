# checkpoint-data-structure-
problem 1 
# Problem 1: Sum of Distinct Elements
def sum_distinct(set1, set2):
    total = 0
    for elem in set1:
        if elem not in set2:
            total += elem
    for elem in set2:
        if elem not in set1:
            total += elem
    return total

# Example usage
set1 = [3, 1, 7, 9]
set2 = [2, 4, 1, 9, 3]
print("Sum of distinct elements:", sum_distinct(set1, set2))  # Output: 13
problem 2 
# Problem 2: Dot Product and Orthogonality
def dot_product(v1, v2):
    ps = 0
    for i in range(len(v1)):
        ps += v1[i] * v2[i]
    return ps

# Example usage
v1 = [1, 2, 3]
v2 = [4, -8, 4]  # Example vectors
if dot_product(v1, v2) == 0:
    print("Vectors are orthogonal")
else:
    print("Vectors are not orthogonal")
