# Web Team Back-End Challenges

Below are a handful of quick challenges for back-end candidiates. Tackle whichever challenge you'd like (unless we asked you to solve a specific challenge).

We use Python pervasively throughout our backend codebase, but use whichever language/framework you feel will solve the challenge effectively.

## Shifted List Search

We have a list of ordered integers (ex: `[1, 3, 7, 8, 9, 10, 11]`). Suppose we slice into that list at a random index and append the "top" half of list to the "bottom" (maintaining the order of both halves while doing so).

**Challenge:** Write a function that returns the largest integer in the "shifted" list.

View the samples below for a better understanding of how the lists are mutated:

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
3. Suppose our initial list contains 1 million elements, is there a more performant way we can find the answer?


## Most Occurring Triplets

Suppose we have a list of tuples representing a web access "log file". Each tuple contains two elements:

1. The path of the request.
2. The ID of the user who made the request.

We want to track user flow through our website; specifically, we want to track "triplets". A triplet is a unique group of three consecutive pages visited by the same user.

**Challenge:** Write a function that returns the 10 most occurring triplets in the log file.

```python
# Here is our log file; essentially a list of tuples.
# Each tuple has two items: `(request_path, user_id)`
log_file = [
    ("/", "user_1"),
    ("/about", "user_1"),
    ("/", "user_3"),
    ("/features", "user_1"),
    ("/about", "user_2"),
    ("/purchase", "user_2"),
    ("/purchase", "user_1"),
    ("/thank-you", "user_1"),
    ("/about", "user_3"),
    ("/thank-you", "user_2"),
    ("/purchase", "user_3"),
    ("/thank-you", "user_3"),
]

# A triplet is a group of three consecutive pages visited by the same user. For example,
# user_1 visited the following pages in this order:
#    "/" , "/about", "/features", "/purchase", "/thank-you"
#
# In this case, user_1 created three unique triplets during her visit:
#    1. ("/", "/about", "/features")
#    2. ("/about", "/features", "/purchase")
#    2. ("/features", "/purchase", "/thank-you")
#
# At the same time, user_3 went through a different workflow but created two unique triplets during his visit:
#    1. ("/", "/about", "/purchase")
#    2. ("/about", "/purchase", "/thank-you")
#
# Your function should return the 10 most occurring triplets in the log file. Given the log file above, the
# returned list should something look like:
#
# [
#    ("/about", "/purchase", "/thank-you"), # cnt 2
#    ("/", "/about", "/features"), # cnt 1
#    ("/about", "/features", "/purchase"), # cnt 1
#    ("/features", "/purchase", "/thank-you"), # cnt 1
#    ("/", "/about", "/purchase"), #cnt 1
# ]
```


