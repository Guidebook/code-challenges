# Guidebook Data Science Intern Challenge

Congratulations on making it to this stage of the interview process! This exercise will test your python coding skills, your data analysis skills, and give you a sense of the kinds of work you would do at Guidebook as a Data Science Intern. In this challenge, you'll first demonstrate your python abilities and perform some specified processing on raw data to produce a dataset. Then, you'll take a deeper look into the dataset you create in part 1 and write up some of your findings.

Please complete all parts to the best of your ability. This should take 1-2 hours to complete.


## Part 1: User Histograms

Often at Guidebook, we aggregate metrics events associated to a user or a guide as a way of describing that entity.
For the first part of this exercise you'll do some of this to demonstrate your Python coding abilities.
Specifically, you are going to write a code which given a list of metrics event dictionaries of form:
```python
[
   {"event": "event name", "properties": {"user_id": 1234}},
   ...
   {"event": "another event name", "properties": {"user_id": 567}}
]
```

creates a data structure of your choosing which keeps track of the number of times each user triggered each event. Furthermore, your solution should not depend on knowing the possible event names in advance. Since this part of the exercise is intended to test your python fundamentals, please stick with the python standard library.

In part 2 you'll take a deeper look at the results from this step, so keep that in mind as you write this out. Once completed, you can import the list `INPUT_DATA` from the included `input_data.py` to create the dataset for part 2. 

### Evaluation for Part 1
For part 1 here we'll be looking mainly at your ability to perform data processing tasks with Python, and more specifically your software writing fundamentals. We won't be grading this as strictly as we would for a software engineering role, but as a team we place high value on readable, maintainable code.


## Part 2: Exploration and Discussion

In the dataset we've given you, there are 4 events: 
- `GuideDownload` which we record every time someone downloads a guide
- `GuideSession` which we record every time a user opens up a guide on their phone
- `ConnectionRequested` which we record every time a user sends a connection request to another user
- `PhotoUpload` which we record every time a guide user uploads a photo to a guide

For the next part of the exercise, let's take a closer look at the `PhotoUpload` event. Using the dataset you created in part 1, what would you tell the team about how users are using this feature?

Please complete a brief write-up of your findings. Include all code needed to reproduce your results, and if you create any plots you'd like to include, please save them as image files in the repo. For this part of the exercise feel free to use any libraries you like. If you run out of time, feel free to mention what you'd like to do and how you'd do it, but make sure to complete and discuss the data exploration steps you think are most important first.

### Evaluation for Part 2
In this section we'll be looking at your data exploration skills, along with your ability to communicate your findings. When looking at these submissions we'll be asking questions like, "How well did this candidate communicate their work?" "How well do they justify their conclusions with the given data?" This exercise is a simplified example of the kinds of problems you'd work on as a Data Science intern at Guidebook and using datasets to tell stories about our platform would be one of the most important things you would do in this role.

