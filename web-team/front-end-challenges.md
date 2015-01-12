# Web Team Front-End Challenges

Below are a handful of code challenges for front-end candidiates. Tackle whichever challenge you'd like (unless we asked you to solve a specific challenge).

We currently use a mix of ReactJS, Backbone, Jquery throughout our codebase (which is almost entirely written in CoffeeScript), but leverage whatever framework(s) you feel will solve the challenge effectively; and be sure to add the logic behind your choice in your project's `README`.


## Autocompleter Challenge

Build an autocompleter input that hits [Guidebook's public search endpoint](https://guidebook.com/om/service/v2/search/?q=foo) and displays the results to the user.

**DOM Assumptions:**

Assume that you have a single `text input` that will allow the user to type strings they wish to search for. You'll be updating elements in an unordered list to reflect the results that are returned from the server.

```html
<input id="search" type="text" placeholder="Search..." />

<ul id="search-results"></ul>
```

**Requirements:**

* Capture key presses from a text input and send async calls to the server sending the current value of the input as the search term.
* The results from each async request should be used to update the unordered list element.
* The url you should make a request to is: https://guidebook.com/om/service/v2/search/?q=foo (where foo is the search string from the input).

**Implementation:**

* Feel free to modify the DOM if you feel you need more specific elements.
* Feel free to use whatever javascript library/framework you wish -- keep in mind that we use ReactJS and Backbone heavily in our codebase.
* Do not take more than 1 hour!
