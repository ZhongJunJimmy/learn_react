# Learning react library

#### Introduction
This is a learning project for react library. It's reference from [React Tutorial From Scratch: A Step-by-Step Guide (2021)](https://ibaslogic.com/react-tutorial-for-beginners/)
#### Basic knowledge:
- nodejs
- javascript

## Start
### What is React?
- It is a JavaScript library
- It was originated at Facebook in 2011 and allow developers to create sizeable web applications or complex UIs by integrating a small and isolated snippet of code.

### Thinking in React Component
- When building an application with React, you build a bunch of independent, isolated and reusable components.
- It like a function that can be reused.

### The Concept of Virtual DOM
1. Real DOM
    - Every time the DOM changes, the browser would need to recalculate the CSS, run layout and repaint the web page.
2. Virtual DOM 
    - Whenever a new element is added to the UI, a virtual DOM is created. Now, if the state of this element changes, React would recreate the virtual DOM for the second time and compare with the previous version to detect which of the virtual DOM object has changed. It then updates ONLY the object on the real DOM.

### Setting up Working Environment
- Require Node 10 or higher
- Though React recommended setting up the environment through the create-react-app CLI tool (coming to that)
`> npx create-react-app <app_name>`

### Using the Create React App CLI
The project path tree view creating by `create-react-app`
```
<app_name>
    ├── node_modules
    ├── public
    │    ├── favicon.ico
    │    ├── index.html
    │    ├── logo192.png
    │    ├── logo512.png
    │    ├── manifest.json
    │    └── robots.txt
    ├── src
    │    ├── App.css
    │    ├── App.js
    │    ├── App.test.js
    │    ├── index.css
    │    ├── index.js
    │    ├── logo.svg
    │    ├── reportWebVitals.js
    │    └── setupTest.js
    ├── .gitignore
    ├── package.json
    ├── README.md
    └── yarn.lock
```
- public: contains the public asset of your application and it is where your static files reside.
- src: working files

### Writing React Directly in HTML
- You’ll have an HTML file where you load three scripts in the head element pointing to their respective CDN – the React, ReactDOM and Babel (An Compiler for javascript).
- ref: [Link](https://codepen.io/ibaslogic/pen/qBaPqBL?editors=1111)

### What is JSX
- This is called JSX (JavaScript XML).
- It is an XML like syntax extension to JavaScript that makes it easier and more intuitive to describe the UI.
- Convert JSX code to plain react code: [Link](https://babeljs.io/repl#?browsers=defaults%2C%20not%20ie%2011%2C%20not%20ie_mob%2011&build=&builtIns=false&corejs=3.6&spec=false&loose=false&code_lz=MYewdgzgLgBApgGzgWzmWBeGAeADgPgAtEEQYB3EAJwQBMBCbAegKA&debug=false&forceAllTransforms=false&shippedProposals=false&circleciRepo=&evaluate=false&fileSize=false&timeTravel=false&sourceType=module&lineWrap=true&presets=env%2Creact%2Cstage-2&prettier=false&targets=&version=7.16.4&externalPlugins=&assumptions=%7B%7D)
- Take note of the following about the JSX:
    - You can use a valid JavaScript expression inside the JSX through curly braces, {}.
    - In JSX, elements attributes, event handlers are always in camelCase. The few exceptions are aria-* and data-* attributes, which are lowercase.
