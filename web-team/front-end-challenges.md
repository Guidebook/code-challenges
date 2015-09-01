# Web Team Front-End Challenges

While we currently use a mix of ReactJS and Backbone throughout our codebase (which is almost entirely written in CoffeeScript), feel free to leverage a modern JS framework (ReactJS, Angular, Ember, etc.) that you feel will address the requirements effectively; and be sure to add the logic behind your choice in your project's `README`.


## Auto-Completer Challenge

Build an auto-completer text input that searches through the list below and displays the results to the user.

**DOM Assumptions:**

Assume that you have a single `text input` that will allow the user to enter strings to search for. You'll be updating elements in an unordered list to reflect the results that are returned from the server.

```html
<input id="search" type="text" placeholder="Search..." />

<ul id="search-results"></ul>
```

**Requirements:**

* Capture key presses from a text input and use the current value of the input to match items in the list (shown below).
* The results from each search should be used to update the unordered list element.

**Implementation:**

* Feel free to modify the DOM if you feel you need more specific elements.
* Feel free to use whatever modern javascript library/framework you wish (don't just do this in jQuery) -- keep in mind that we use ReactJS and Backbone heavily in our codebase.
* Do not take more than 1 hour!


**The List:**

Search through this list for approximate matches. For example, if the user enters `san`, it should match `san`, `santiago`, `san francisco`, `santa rosa`, etc. If they enter `sant`, it should only match `santiago` and `santa rosa`.

```javascript
[
  'san', 'san jose', 'santiago', 'san francisco', 'santa rosa', 'san juan', 'sabadell', 'salamanca', 'salt lake city', 'salinas', 'salem', 'sausalito', 'taipei', 'tel aviv', 'tempe', 'termez', 'temuco', 'tiajuna', 'tieling', 'thousand oaks', 'thunder bay', 'tokyo', 'tulsa'
]
```
