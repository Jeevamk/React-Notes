# Q: What is `SPA` (Single page application)
-A single-page application (SPA) is a webpage that dynamically interacts with the web browser by rewriting the current web page with data from the webserver. As a result, the webpage does not reload during its execution and instead operates in a browser.

# Q: What is the difference between Single Page applications and Multi Page applications?
-Single-page Applications are perfect for creating dynamic, fast-loading websites, especially if you are designing to create a mobile app. The biggest downside of this model is that it has poor search engine optimization and is ranked lower in search engines. Therefore, it is ideal for social networks, private groups, and SaaS applications where SEO is not required. Gmail, Google Maps, Facebook, and GitHub are among the examples.
-Multi-Page Applications are valuable for online stores, catalogs, and commercial websites because they can handle large amounts of data that require several pages, features, and menus.

# Q: What are the advantages of a single-page application?
1) All webpage resources are loaded only once throughout the application because SPA is faster, and data is the sole resource that is sent.
2) SPA effectively caches local storage because it sends only one request, retains all of the data, and uses it even when offline.

# Q: Disadvantanges?
-SEO difficulties: Any web app is written in JavaScript loads data without reloading the page and only when the user requests it. This means there are no specific URLs optimized for search engines, and the content is not visible to search engines. The problem can only be solved by server-side rendering.

# Q: `CDN` (Content Delivery Network)
- Distributed network of servers to deliver web content.
- it is a URL that point to resoucers.
- It is a website that already hosted by developers , as we need that we can fetch the content from that.

 # Q: `How CDN Works`
-When you visit a website, your browser sends a request to the website's server to retrieve the necessary files (HTML, CSS, JavaScript, images, etc.) to display the webpage.
-With a CDN in place, instead of fetching all the content from the original server, the request is routed to the nearest server within the CDN network.
-The CDN server caches (stores) copies of the website's content, so if another user requests the same content, it can be delivered quickly from the server closest to them.
-This reduces latency (the time it takes for content to load) because the data travels a shorter distance, resulting in faster loading times for users.

# Q: `Npm`
- Package manager.
- it manages all the packages. (Packages itclude libraries and frameworks)
- -It is default package manager of node.js

# Q: `package.json`
  - It is a configuration of NPM
  - it is json format.
  - It contain meta data about the project and dependencies
  - It take on the versions.
  - One of the key sections of package.json is the "dependencies" object, which lists the packages that your project depends on to run correctly.

 
# Q: `package-lock.json`
   -package-lock.json is a file automatically generated by npm that serves as a record of the exact versions of dependencies installed in a project.

# Q: `dependencies`
  -Dependencies are packages that your project relies on to run correctly. These can be libraries, frameworks, utilities, or any other code modules.
  - it is required in production enviornment.
   
# Q: `devdependencies`
   -devDependencies are packages that are only needed during development or for building/testing purposes, but not in production.

# Q: `Bundlers` (e.g., webpack, Parcel):
-Bundlers are tools that take multiple JavaScript files and their dependencies and bundle them together into a single file (or multiple files) for optimized delivery to the browser.

# Q: `Transpilers` (e.g., Babel):
-Transpilers are tools that convert source code written in one programming language or version into another language or version. In the context of JavaScript development, transpilers are primarily used to convert modern JavaScript code (ES6+ syntax) into older versions of JavaScript (ES5) that are compatible with older browsers. 

# Q: `React Element`:
-A React Element is a plain JavaScript object that represents a single node in the Virtual DOM tree.
-React Elements are lightweight and immutable, meaning they cannot be modified once created.
-You create React Elements using JSX syntax or React.createElement() function, specifying the type of element.

# Q: `State`:
-<b>State is a javascript object that can store the data or information related to react component and it can used to store, manage and update the data within the application.<b><br>
-It allow for dynamically changes the user interface.<br>
-State represents the internal data of a component that can change over time.
-Unlike props, which are passed down from parent components and are immutable, state is managed internally by the component and can be modified using the setState() method.
-Changes to the state trigger re-rendering of the component, updating the UI to reflect the new state.
-State is typically initialized in the constructor of a class component or using the useState() hook in functional components.

# Q: `Props`:
-Props (short for properties) are inputs to a component that are passed from its parent component.
-Props allow you to customize the behavior and appearance of a component by passing data or functions as arguments.
-Props are read-only and cannot be modified by the component itself. They are used to pass data from parent to child components.
-In functional components, props are received as arguments to the component function. In class components, they are accessed using this.props.

# Q: Difference between `React` and `ReactDOM`
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

A: In React version 16.8, React introduced a new pattern called Hooks. React Hooks are simple JavaScript functions that we can use to isolate the reusable part from a functional component.<br>-Hooks can be stateful and can manage side-effects.<br>
-Hooks allow you to reuse stateful logic without changing your component hierarchy. This makes it easy to share Hooks among many components or with the community.<br>
-It access events and lifecycle methods to function components.

# Q: Why do we need `useState Hook`?

A:-It is used to create state variables.<br>
-Whenever the state variable is update react will re-render the component.<br> 
-useState hook is used to maintain the state in our React application. <br>
-It accept a initial state and return 2 values<br>
         - Current value<br>
         - Function that updated the state <br>
-It keeps track of the state changes so basically useState has the ability to encapsulate local state in a functional component.<br>
-The useState hook is a special function that takes the initial state as an argument and returns an array of two entries.<br>
-UseState encapsulate only singular value from the state, for multiple state need to have useState calls.

# Q:useEffect()
 - It allow you to perform side effects in functional component.<br>
 - It accept a function as it first argument and a optional array of dependencies as it second argument.<br>
 - If any of the dependencies changes between the render, the effect will re run.If the array is omited , the effect runs after every render.

# Q: `Components`
A: * Independent and reusable bit of code.
   * It is a (small chunk) part of user Interface in a webpage.
   * Same purpose of js functions.
   * It's primary job is render it's user interface and update whenever the internal state is changed.
   * It manage events.
   * It accepet input as a props and return react element.

  2 types of components,
    1) Class Components (state component)- * Components are defined as ES6 classes and provide life cycle methods and state.<br>
                          * It define a class that extends the base React.Component and impliments the `render()` method that `return` the markup of the component.<br>
    2) Function Components (stateless component) - It defined as js functions. It accept input as a props and return JSX.It do not have state.<br>
                                                   * After the introduction of hooks , which allow function component to have local state and access life cycle method.<br>

# Q: `Pure component`
- It is a specific implimentation of react component.<br>
- It automatically impliment "shouldComponentUpdate()" method , with shallow comparison of state and props.If there are no change in shallow comparison it does not re render.<br>
- Shallow comparison indicate that if there is no change in the props and states then react skip the rendering process of that component.<br>
- It can improve the performance by preventing unnecessary re renders.

# Q: `Higher order component`
- Higher order components are the function that take component and return a new component with additional functionality.<br>
- It allow you to reuse the component logic across multiple component without repeating code.
- code reusability and modularity of react applications.

# Q: `Context Component`
- It provide a convenient way to manage global state and share data across the component tree without having to pass props down manually at every level.<br>
-Context is created using the `React.createContext` method and is then provided to the React tree using the `Context.Provider` component. The context values can be consumed by any component 
 within the tree using the `Context.Consumer` component or the `useContext` hook.


# Q: Types of hooks
-useState()
-useEffect()
-useContext()
-useRef()
-useReducer()
-useCallback()
-useMemo()
-custom hooks





 
