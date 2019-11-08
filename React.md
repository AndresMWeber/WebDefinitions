# REACT

* **react-dom** - serves as the entry point to the DOM and server renderers for React
* **react-router** - Core navigation lib
* **react-router-dom** - Navigation for dom-based apps
* **react-router-native** - Navigation for react-native apps
* **react-router-redux** - Bindings between redux and react router
* **react-redux** - redux interface for react components

## React Properties

* **Declarative** - In react the DOM is declarative. This means we never interact with DOM, the UI is updated when we change the state. This makes it easier to design UI and debug them, You can just change the program's state and see how the UI will look at that particular time.

* **Component Based** - Conceptually, components are like JavaScript functions. They acce
pt arbitrary inputs (called “props”) and return React elements describing what should appear on the screen.

* **JSX** - JSX is an XML/HTML-like syntax used by React that extends ECMAScript so that XML/HTML-like text can co-exist with JavaScript/React code. The syntax is intended to be used by preprocessors (i.e., transpilers like Babel) to transform HTML-like text found in JavaScript files into standard JavaScript objects that a JavaScript engine will parse.

* **React Native** - React Native is a framework for building native applications using JavaScript. React Native compiles to native app components, which makes it possible for you to build native mobile applications. In React JS, React is the base abstraction of React DOM for the web platform, while with React Native, React is still the base abstraction but of React Native. So the syntax and workflow remain similar, but the components are different.

* **Single-Way data flow**
  * state is passed to the view and to child components
  * actions are triggered by the view
actions can update the state
the state change is passed to the view and to child components

* **Functional Components** (aka stateless components) - A functional(a.k.a. stateless) component is just a plain javascript function which takes props as an argument and returns a react element.

* **Class Components** (aka stateful components) - Class syntax is one of the most common ways to define a React component. While more verbose than the functional syntax, it offers more control in the form of lifecycle hooks.

#### Functional vs Class based Components
* Class based components
  * state
  * lifecycle methods
  * memoization with React.PureComponent
* Functional components:
  * state (useState, useReducer hooks)
  * lifecycle methods (via the useEffect, useLayoutEffect hooks)
  * memoization via the memo HOC

**Uncontrolled vs Controlled Components** -  In a controlled component, form data is handled by a React component. The alternative is uncontrolled components, where form data is handled by the DOM itself. To write an uncontrolled component, instead of writing an event handler for every state update, you can use a ref to get form values from the DOM.

**Lifecycle Methods** - React components all have their own phases.  React provides built-in methods on the React Component that allow you to inject your own functionality into those phases.

**Hooks** - They let you use state and other React features without writing a class. Hooks are backwards-compatible.

**Reason for (htmlFor, className)** - These are old issues based on early React that would evaluate the javascript protected keywords as real JS syntax.  It is no longer an issue, but will give you a warning.  (This might be changed in future versions of React)

**Reason for key prop in list of render components** - Key is used to look at the dom and see if the same rendered component is findable in the rendered DOM to reduce recreation of dom elements and increase efficiency/reduce adding/removing elements from/to the DOM.

**React Refs** - In the typical React dataflow, props are the only way that parent components interact with their children. To modify a child, you re-render it with new props. However, there are a few cases where you need to imperatively modify a child outside of the typical dataflow. The child to be modified could be an instance of a React component, or it could be a DOM element.

  * Usage example: On image load callback to a DOM img tag element to resize/affect grid position/spacing aka affecting React Component DOM elements based on DOM events.

    1. ``` React.createRef()``` in constructor
    1. Add ```ref=(instance property ref was stored in)``` to property of the jsx dom element


## React Routing

Anchor Tag Usage - Never use this while using react-router because this dumps all React/Redux state data when directing to the new path based on a new http request..  It is also dumping all JS data/variables that were stored on the current page..

* **BrowserRouter** - Uses everything after **TLD** (**.com, .net**) as the path. (*page.com/pagetwo*)
* **HashRouter** - Uses everything after # as the **URL** path. (*page.com/#/pagetwo*)
* **MemoryRouter** - Does not use the **URL** to track navigation. (*page.com*)