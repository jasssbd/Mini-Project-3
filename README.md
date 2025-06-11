# Mini-Project-3
subset selection problem
from itertools import combinations

# Given set
numbers = {-12, -3, -6, 7, 2, -2, 6, 3, 9, -7, -5, -8, 1, 11, -9, -4}

# Convert to list for combinations
num_list = list(numbers)

# Find all subsets of size 5 whose sum is 0
result = [subset for subset in combinations(num_list, 5) if sum(subset) == 0]

# Print the results
print("Subsets of size 5 with sum = 0:")
for r in result:
    print(r)
