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
REACT AND REACTDON
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

------------
