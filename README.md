# React-Q-A ⁉
---------
LIBRARY AND FRAMEWORK
---------
- What is library and framework :- <br />
     Both frameworks and libraries are code written by someone else that is used to help solve common problems. <br />
     - Library : - <br />
          Library is a collection of pre writened code that you can to perform specific task . <br />
     - Framework : - <br />
          Framework is a structure that you can build softwere on
- Differents between library and framework :- <br />
     Inversion of control :- When you use a library, you are in charge of the flow of the application. You are choosing when and where to call the library. When you use a framework, the framework is in charge of the flow. It provides some places for you to plug in your code, but it calls the code you plugged in as needed.
---------
SPA
---------
- What is SPA ?  <br />
     A single-page application (SPA) is a webpage that dynamically interacts with the web browser by rewriting the current web page with data from  the webserver. As a result, the webpage does not reload during its execution and instead operates in a browser.If any changes occur in current page its only re render that element only does not reload entire page. it is cleint side rendering . Single-page Applications are perfect for creating dynamic, fast-loading websites <br />
- Difference between Single page application and multy page application :- <br />
     ▶ User experience : - <br />
               SPA provoid smoother and more responsive user experience since they only update portion of the page that have chenged , resulting the faster navigation and reduced latency .<br />
               MPA may have slower performance due to reload entire page <br />
     ▶ Performance : - <br />
               SPA only fetch and render the neccessory data for each interaction so its tend to be efficient in data transfer and server load. <br />
               MPA may reqiure serve to genarate and serve complete HTML page for each request so its take higher serve load and slower performance
     ▶ Development : - <br />
               SPA can be more complex to develop and maintain , Especially for large application due to the need for client-side routing , state management and asynchronous data handling <br />
               MPA is easier or simpler development required , they follow more treditional server-side rendering approach <br />
     ▶ Search Engine Optimisation (SEO) : - <br />
               SPA initially faced challanges with SEO due to client-side render <br />
               MPA have better SEO since search engine can simply find and index individual HTML page
----------
CDN
----------
- What is content delivery (distribution) network (CDN) ? <br />
     A system of distributed servers that deliver web condent to users based on their geographical locations. <br />
- How the CDN work ? <br />
     When a user requests content from the website, the CDN dynamically determines the user's location and routes the request to the nearest server in the network. Then the server delivers the content to the user, <br />
----------
EMMET
----------
- What is "Emmet" ? <br />
     Emmet is essential toolkit for web-developers . It allows you to 'type shortcut' that are then expanded into full pieces
----------
CROSSORIGIN
----------
- What is `crossorigin in script tag`?  <br />
     crossorigin attribute is used to share the resources from one domain to another domain. Basically, it is used to handle the CORS request . That checks whether it is safe to allow for sharing the resources from other domains.
----------
REACT
----------
- What is REACT ?
       React is an open source javascript front-end library use to create interactive user interfaces (UI) . Especially for single page applicaiton , its creted by Jordan Walke from facebook in 2011 . React allows developers to leverage small modules or components to develop the entire UI.
- Features of react <br />
       🚀 Modularity and scalability <br />
       🚀 Faster rendering process <br />
       🚀 Enhanced code structure stability <br />
       🚀 Easy to use and learn <br />
       🚀 Code reusability <br />
----------
REACT AND REACTDOM
----------
- Difference between react and react dom ? <br />
     React is a javascript library for creating interactive user interfaces<br />
     React DOM is also a javascript library that allow react to interact with the DOM  <br />
     Whenever we use component, classes, elements, etc. We’re using React <br />
     whenever we use methods like render() or findDOMNode() we’re using React-DOM.
------------
REACT ELEMENT
------------
- What is react element ? <br />
     it is an object representation of a virtual DOM node. Elements are the smallest building blocks of React apps. An element describes what you want to see on the screen. A React element is a lightweight, immutable object representation of a component's structure and properties. These elements are not actual DOM elements; instead, they are virtual representations of UI components. React elements are ultimately transformed into actual DOM elements and rendered onto the screen by the React rendering engine.<br />
- How to create react element ? <br />
     We can create with 2 types <br />
     first<br />
     ----- <br />
  Import React from "react" then => const elem => call React.createElement() function . it take 3 arguments <br />
     - Tag
     - Attributes
     - Children
       eg : - const elem = React.createElement("h1",{},"Hello world !!") <br />
            nb :- {} take attributes eg :- {style:{color:"red"}} <br />
       Second<br />
       ------<br />
  We can create react element using jsx in simply <br />
       eg : - <br />
       const elem = "<h1 Hello world !! /h1>"
------------
VIRTUAL DOM
------------
- What is actual dom or real dom ? <br />
     The Real DOM, also known as the actual DOM, is the browser’s representation of a web page’s HTML structure. When a user interacts with a web page, such as clicking a button or filling out a form, the browser updates the Real DOM to reflect the changes. The browser then re-renders the page to display the updated HTML. <br />
- What is virtual dom ? <br />
     It is the javascript object representation of actual dom .  The Virtual DOM is a lightweight copy of the Real DOM, which allows for faster updates and improved performance. When a user interacts with a web page, React updates the Virtual DOM, compares it with the previous version, and only updates the Real DOM with the necessary changes. This process is known as Reconciliation.
- Differences between real dom virtual dom ?<br />
     -the Real DOM is much slower than the Virtual DOM, as every update requires the browser to recalculate the entire document layout. On the other hand, the Virtual DOM is a lightweight copy of the Real DOM, which allows for faster updates and improved performance.<br/>
     - the Real DOM is a tree structure, and every node has an attached event listener. When a user interacts with a web page, the browser executes the corresponding event listeners. This process can be slow and resource-intensive. In contrast, the Virtual DOM updates are more efficient, as event listeners are only attached to the root node and not every individual node <br/>
------------
COMPONENT
------------
- What is component ? <br />
     Components are independent and reusable bits of code. They serve the same purpose as JavaScript functions. component is a javascrpt class or functions that accept input as props and return react elements that describe how a section of UI should appear <br />
- What are the types of component ? <br />
     - Class component :- <br />
          This components are defined in javascript es6 classes , its provoid life cycle method and state <br />
     - Function component :- <br />
          This components are javascript functions and donot have their own state, but they can receive and render props.<br />
- Other types of components ? <br />
     - Pure component :- <br />
     - Stateless function components :- <br />
     - Higher order components :- <br />
     - Context components :- <br />
- What is pure component ? <br/>
     Pure component is a specific implimentation of react component . It automatically impliment a "shouldComponentUpadte()" method , This method with a shallow comparison of sates and props. If there are no changes dettermine in shallow comparison , the component will not re-render<br />
       - The shallow comparison checks for differences at the top level of the props and state objects <br />
       - If the shallow comparison indicates that the props and state have not changed, React skips the rendering process for that component, <br />
       - optimizing performance by preventing unnecessary re-renders. <br />
- What is state less function component ? <br />
     It refers to function component , That does not have their own internal state , its known as functional component, Functional components are defined as JavaScript functions that accept props as input and return React elements to describe what should be rendered on the UI. <small>With the introduction of React hooks in React 16.8, functional components gained additional capabilities, such as the ability to manage state and side effects using hooks like useState, useEffect, and others. This made functional components more versatile and capable of handling complex logic previously reserved for class components.</small>
- What is stateful component ?<br />
     A "stateful component" in React refers to a class component that manages its own internal state. Unlike stateless functional components,tateful components have the ability to maintain and update their state independently.
- What is higher order component ?<br />
     Higher Order Components in React are functions that take a component and return a new component with enhanced functionality. This pattern allows for the reuse of component logic across multiple components without repeating code. <small>Higher Order Components in React are functions that enhance the functionality of components by wrapping them with additional logic or behavior, promoting code reusability and modularity in React applications.</small>
- what is context component ? <br />
      context components provide a convenient way to manage global state and share data across components in a React application, enhancing code organization and reducing the need for prop drilling.
----------
STATE AND PROPS
----------
- What is state and props ? <br />
     state and props both are fundamental concept using for managing and passing data from one component to another, but they have different functions and characteristics.<br />
  PROPS (Properties):- <br />
       - Props are short for "properties" and are a mechanism for passing data from parent to child component in react <br />
       - Props are immutable . Meaning they canot modified by the component that receives them. <br />
       - They contain any type of data such as array,string,number or a jsx elements too. <br />
       - Component only can pass props on a unidirectional manner, where data flow frm parent to child only . <br />
       - example :- <Component propsName = {Props value} /> <br />
  STATE :- <br />
       - In react , state is a normal javascript object , that store data or informations related to react component. It can be used for store,manage and update data with in the application , it allow for dynamic changes to user inteface. <br />
---------
HOOKS
---------
- What is hooks ?<br/>
     Hooks in React are functions that enable functional components to have stateful logic and interact with React features that were previously only available in class components. <br />
- useState :- <br />
     used for managing states within the functional components. States are used to manage and store some data within a component.<br />
- useEffect :- <br />
     useEffect is a built-in hook in React that allows functional components to perform side effects. Side effects are actions that occur outside the scope of the component rendering, <br />
- useContext :- <br />
      Context allows you to pass data through the component tree without having to pass props manually at every level. It's particularly useful for sharing state or other data between components that are not directly related in the component tree. <br />
