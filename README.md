# Q: What is SPA (Single page application)
-A single-page application (SPA) is a webpage that dynamically interacts with the web browser by rewriting the current web page with data from the webserver. As a result, the webpage does not reload during its execution and instead operates in a browser.

# Q: What is the difference between Single Page applications and Multi Page applications?
-Single-page Applications are perfect for creating dynamic, fast-loading websites, especially if you are designing to create a mobile app. The biggest downside of this model is that it has poor search engine optimization and is ranked lower in search engines. Therefore, it is ideal for social networks, private groups, and SaaS applications where SEO is not required. Gmail, Google Maps, Facebook, and GitHub are among the examples.
-Multi-Page Applications are valuable for online stores, catalogs, and commercial websites because they can handle large amounts of data that require several pages, features, and menus.

# Q: What are the advantages of a single-page application?
1) All webpage resources are loaded only once throughout the application because SPA is faster, and data is the sole resource that is sent.
2) SPA effectively caches local storage because it sends only one request, retains all of the data, and uses it even when offline.

# Q: Disadvantanges?
-SEO difficulties: Any web app is written in JavaScript loads data without reloading the page and only when the user requests it. This means there are no specific URLs optimized for search engines, and the content is not visible to search engines. The problem can only be solved by server-side rendering.

# Q: CDN (Content Delivery Network)
- Distributed network of servers to deliver web content.
- it is a URL that point to resoucers.
- It is a website that already hosted by developers , as we need that we can fetch the content from that.

 # Q: How CDN Works
-When you visit a website, your browser sends a request to the website's server to retrieve the necessary files (HTML, CSS, JavaScript, images, etc.) to display the webpage.
-With a CDN in place, instead of fetching all the content from the original server, the request is routed to the nearest server within the CDN network.
-The CDN server caches (stores) copies of the website's content, so if another user requests the same content, it can be delivered quickly from the server closest to them.
-This reduces latency (the time it takes for content to load) because the data travels a shorter distance, resulting in faster loading times for users.

# Q: Npm
- Package manager.
- it manages all the packages. (Packages itclude libraries and frameworks)
- -It is default package manager of node.js

# Q: package.json
  - It is a configuration of NPM
  - it is json format.
  - It contain meta data about the project and dependencies
  - It take on the versions.
  - One of the key sections of package.json is the "dependencies" object, which lists the packages that your project depends on to run correctly.

 
# Q: package-lock.json
   -package-lock.json is a file automatically generated by npm that serves as a record of the exact versions of dependencies installed in a project.

# Q: dependencies
  -Dependencies are packages that your project relies on to run correctly. These can be libraries, frameworks, utilities, or any other code modules.
  - it is required in production enviornment.
   
# Q: devdependencies
   -devDependencies are packages that are only needed during development or for building/testing purposes, but not in production.

# Q: Bundlers (e.g., webpack, Parcel):
-Bundlers are tools that take multiple JavaScript files and their dependencies and bundle them together into a single file (or multiple files) for optimized delivery to the browser.

# Q: Transpilers (e.g., Babel):
-Transpilers are tools that convert source code written in one programming language or version into another language or version. In the context of JavaScript development, transpilers are primarily used to convert modern JavaScript code (ES6+ syntax) into older versions of JavaScript (ES5) that are compatible with older browsers. 

# Q: React Element:
-A React Element is a plain JavaScript object that represents a single node in the Virtual DOM tree.
-React Elements are lightweight and immutable, meaning they cannot be modified once created.
-You create React Elements using JSX syntax or React.createElement() function, specifying the type of element.

# Q: State:
-State represents the internal data of a component that can change over time.
-Unlike props, which are passed down from parent components and are immutable, state is managed internally by the component and can be modified using the setState() method.
-Changes to the state trigger re-rendering of the component, updating the UI to reflect the new state.
-State is typically initialized in the constructor of a class component or using the useState() hook in functional components.

# Q: Props:
-Props (short for properties) are inputs to a component that are passed from its parent component.
-Props allow you to customize the behavior and appearance of a component by passing data or functions as arguments.
-Props are read-only and cannot be modified by the component itself. They are used to pass data from parent to child components.
-In functional components, props are received as arguments to the component function. In class components, they are accessed using this.props.

# Q: Difference between React and ReactDOM
-React is the core library for building user interfaces in React applications, providing features like component-based architecture, state management, and JSX syntax.
-ReactDOM is a package specifically for interacting with the DOM, providing methods for rendering React components into the browser, hydrating server-rendered content, handling events, and 
 more.

 # Q: What is `Parcel/Webpack`? Why do we need it?

-Parcel and webpack are the bundlers used mostly for JavaScript or Typescript code that helps you to minify, clean, and make your code compact so that it becomes easier to send a request or receive the response from the server when it usually takes you to transfer multiple files without using any bundler for loading the page of your application. Both of these bundlers substantially reduce the time it takes for the transfer of data and files to the server from the application. Along with that both bundlers parcel and webpack remove the unnecessary comments, new lines, any kind of block delimiters, and white spaces while the functionality of the code remains unchanged.

-Use of Parcel/Webpack:
Module bundlers are the way to organize and combine many files of JavaScript code into one file. A JavaScript bundler can be used when your project becomes too large for a single file or when you're working with libraries that have multiple dependencies.

# Q: Is `JSX` mandatory for React?

-JSX is an Extension Syntax that allows writing HTML and Javascript together easily in React and is used to create React elements. These elements are then rendered to the React DOM. Each JSX element is just to make use of React easy and for calling React.createElement(component, props, …children) with less work. So, anything that is done with JSX can also be done with just plain JavaScript. So  JSX is not mandatory but is used for writing better and clean code instead of writing code using React.CreateElement.

# Q: Is `ES6` mandatory for React?

ES6 is not mandatory for `React` but is highly recommendable. The latest projects created on React rely a lot on ES6. React uses ES6, and you should be familiar with some of the new features like: Classes, Arrow Functions, Variables(let, const).
ES6 stands for ECMAScript 6. ECMAScript was created to standardize JavaScript, and ES6 is the 6th version of ECMAScript, it was published in 2015.

# Q: What is `<React.Fragment></React.Fragment>` and `<></>`?

<React.Fragment></React.Fragment> is a feature in React that allows you to return multiple elements from a React component by allowing you to group a list of children without adding extra nodes to the DOM.
<></> is the shorthand tag for React.Fragment. The only difference between them is that the shorthand version does not support the key attribute.

# Q: What are `React Hooks`?

A: In React version 16.8, React introduced a new pattern called Hooks. React Hooks are simple JavaScript functions that we can use to isolate the reusable part from a functional component. Hooks can be stateful and can manage side-effects.
Hooks allow you to reuse stateful logic without changing your component hierarchy. This makes it easy to share Hooks among many components or with the community.

# Q: Why do we need `useState Hook`?

A: useState hook is used to maintain the state in our React application. It keeps track of the state changes so basically useState has the ability to encapsulate local state in a functional component.
The useState hook is a special function that takes the initial state as an argument and returns an array of two entries. UseState encapsulate only singular value from the state, for multiple state need to have useState calls.



 
