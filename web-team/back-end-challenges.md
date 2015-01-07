# Web Team Back-End Challenges

Below are a handful of quick challenges for back-end candidiates. Tackle whichever challenge you'd like (unless we asked you to solve a specific challenge).

We use Python pervasively throughout our backend codebase, but use whichever language/framework you feel will solve the challenge effectively.

## Algorithm Challenges

### Sliding Number Search

We have a list of ordered integers (ex: `[1, 3, 7, 8, 9, 10, 11]`). Suppose we slice into that list at a random index and shift the "top" part of list to the "bottom" (maintaining the order of both halves of the list). Check the samples below for a better understanding of how the lists are mutated.

**Challenge:** Write a function that returns the largest integer in the "shifted" list.

```python
# Sample 1
initial_list = [1, 3, 7, 8, 9, 10, 11]  # Here is our initial ordered list
shifted_list = [8, 9, 10, 11, 1, 3, 7]  # Here is the list after it has been sliced (at index 3) and shifted
# Your function should return `11`

# Sample 2
initial_list = [2, 4, 6, 8, 10]  # Here is our initial oredered list
shifted_list = [6, 8, 10, 2, 4]  # Here is the list after it has been sliced (at index 2) and shifted
# Your function should return `10`

# Sample 3
initial_list = [2, 4, 6, 8, 10]  # Here is our initial oredered list
shifted_list = [2, 4, 6, 8, 10]  # Here is the list after it has been sliced (at index 0) and shifted
# Your function should return `10`
```

1. Can you identify any edge cases that we need to account for?
2. Can you explain the orders of growth implications of the algorithm you implemented?
3. Suppose our initial list contains 1 million elements, is there a faster way we can find the answer?

### Most Occuring Triplets




## Django Specific Challenges

###