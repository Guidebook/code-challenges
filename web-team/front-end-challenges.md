# Frontend End Challenges

## Autocomplete Challenge
Currently we're using  [React](https://facebook.github.io/react/) throughout our codebase (which is written in ES6 Javascript).

We don't want to ask you abstract technical questions during the iterview, so we have a small challenge for you.

Build a React application that lets users search for a city in a provided list.

1. Capture key presses from a text input and use the current value of the input to match items in the list (shown below).
2. The application should output the results under the input field as soon as you type at least 3 characters.
3. If you type less than 3 characters in the text field, it should not output any results. (It can return a prompt to type more at least 3 characters)
4. If there are no results for the search, you should let the user know.
5. Search through this list for approximate matches. For example, if the user enters `san`, it should match `san`, `santiago`, `san francisco`, `santa rosa`, etc. If they enter `sant`, it should only match `santiago` and `santa rosa`.
6. When the page loads the search field should be selected automatically, so you can start typing (similar to when you go to https://www.google.com/)

**The City List:**

```javascript
const cities = [
  'san', 'san jose', 'santiago', 'san francisco', 'santa rosa', 'san juan', 'sabadell', 'salamanca', 'salt lake city', 'salinas', 'salem', 'sausalito', 'taipei', 'tel aviv', 'tempe', 'termez', 'temuco', 'tiajuna', 'tieling', 'thousand oaks', 'thunder bay', 'tokyo', 'tulsa'
]
```

### Build setup
This coding challenge is not in place to evaluate how you set up your React / Babel / Webpack build, but to give you a chance to build something small so we can see how you approach it.
In order to adhere to the 2-3 hour target time, we *highly* recommend that you use [create-react-app](https://github.com/facebookincubator/create-react-app).
After following the instructions (if you get stumped or confused, please feel free to reach out to the hiring manager for the role), edit `App.js` and add any files to complete the challenge as you see fit.

### Requirements
- Use [React](https://facebook.github.io/react/)
- Provide a `README` file and add information on how to build and/or run the project locally. This file can also include your thought process and any explanation.
- Push the application to a public github repo and provide us with a link.

### Implementation
- If you want to, feel free to use any boilerplate projects and `gulp`, `grunt`, `webpack` that bootstap the project for you, (but we recommend [create-react-app](https://github.com/facebookincubator/create-react-app), as noted above).
- If you are using any js processors, **include both source and distribution files**.
- Add some styles, make it pretty.
- Do not cheat. There are lots of autocomplete projects out there, we're not interested in those. We want to see **how you think**.
- If you want to go above and beyond, by adding additional functionality such as some sort of list view that shows your selected cities or a more advanced autocomplete feel free to, **as long as you still satisfy the original requirements**.

### What we're evaluating
- Is there enough information for us to run the project?
- Does it work?
- How are the components structured?
- How clean is the code?
- How does using it feel overall?

### Timeframe
Take as much time as you need. We're expecting this will take you one or two evenings. (Somewhere up to 2-3 hours if you're new to React.)

### More Questions?
Contact your assigned developer.
