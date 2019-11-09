
# JavaScript Terms/Concepts

# Contents
[`JavaScript Terms/Concepts`](#javascript-termsconcepts)

[`Contents`](#contents)

[`ECMAScript`](#ecmascript)

[`History of ECMAScript versions`](#history-of-ecmascript-versions)

[`Definitions`](#definitions)

[`Types of Authentication`](#types-of-authentication)

[`4 Patterns of Function Invocation`](#4-patterns-of-function-invocation)

[`4 Principles of OOP`](#4-principles-of-oop)

[`Javascript Modules`](#javascript-modules)

[`Types of Web Development Stacks`](#types-of-web-development-stacks)

<hr style="page-break-before:always;display:none;">

## ECMAScript
**ES# (ECMAScript)** is a just a standard created to standardize JS across all browsers.  ES# releases are just versions of that standard.

#### History of ECMAScript versions:
    * 1st Edition (1997)
    * 2nd Edition (1998)
    * 3rd Edition (1999)
    * 4th Edition (abandoned)
    * 5th Edition (2009)
    * 5.1 Edition (2011)
    * 6th Edition - ECMAScript 2015
    * 7th Edition - ECMAScript 2016
    * 8th Edition - ECMAScript 2017
    * 9th Edition - ECMAScript 2018
    * 10th Edition - ECMAScript 2019

[`^ Back to Top`](#contents)

## Definitions
**Immediately-invoked function expression** (**IIFE**) -  is a JavaScript design pattern which produces a lexical scope using JavaScript’s function scoping.

* avoid variable hoisting from within blocks
* protect against polluting the global environment and
* simultaneously allow public access to methods while retaining privacy for variables defined within the function

**Rest Pattern (ES6)** - allows you to spread as many components of a container into variables and catch the “rest” of the container’s components you did not specify variables for.

**Spread (ES6)** - allows you to expand something that is currently grouped inside a particular container and assign it to a different container

**for/in Loop (ES 1st Edition)** - When using for/in loops with arrays, it is important to note that the “key” of an array is just the index. So when using a for/in loop with an array you will not get the value at each index, instead, you will get the index.

**for/of Loop (ES6)** - a recent addition that is specifically intended to iterate over iterable objects, like arrays, strings, maps, and sets. Syntactically, it is almost identical to the for/in loop except you replace in with of. Functionally they are different. Instead of getting the key, like the for/in loop, you get the actual value at that location.

**Destructuring Assignment** - Taking an array/object and splitting its component indices and storing into receiving variables.

&nbsp;&nbsp;```const [first, second, ...rest] = ['some', 'long', 'array', 'of', 'values']```

**Anonymous closure** - these functions have its own evaluation environment or “closure”, and then we immediately evaluate it. This lets us hide variables from the parent (global) namespace.

**Module pattern** - was used to mimic the concept of classes (since JavaScript doesn’t natively support classes) so that we can store both public and private methods and variables inside a single object.

**Hoisting** - Hoisting is JavaScript's default behavior of moving all declarations to the top of the current scope (to the top of the current script or the current function).  JavaScript only hoists declarations, not initializations.

**Promise (ES2015)** - A Promise is an object representing the eventual completion or failure of an asynchronous operation. Essentially, a promise is a returned object to which you attach callbacks, instead of passing callbacks into a function.

**Arrow Function (ES6)** - These are anonymous functions with their own special syntax that accept a fixed number of arguments, and operate in the context of their enclosing scope — ie the function or other code where they are defined.

**Node Require vs Import (ES2015)** - Require can be called within a scope, but import can only be called in the global scope, therefore reducing a lot of pressure on transpilers that cannot introspect/tree shake properly in that situation.

**Polyfill** - In web development, a polyfill is code that implements a feature on web browsers that do not support the feature. Most often, it refers to a JavaScript library that implements an HTML5 web standard, either an established standard (supported by some browsers) on older browsers, or a proposed standard (not supported by any browsers) on existing browsers. Formally, "a polyfill is a shim for a browser API"

**Isomorphic/Universal JavaScript** - Made popular by Spike Brehm of AirBnB, means rendering pages on both the server and client side. It usually implies the use of JavaScript and Node.js/Io.js because they allow for the re-use of libraries, allowing browser JavaScript code to be run in the Node.js/Io.js environment with very little modification. As a result of this interchangeability, the Node.js and JavaScript ecosystem supports a wide variety of isomorphic frameworks such as React.js, lazo.js, and Rendr amongst others.

<p align="center">
    <img src=https://raw.githubusercontent.com/AndresMWeber/WebDefinitions/master/media/14_isomorphic.png>
</p>

**Strict Mode** - JavaScript's strict mode, introduced in **ECMAScript 5**, is a way to opt in to a restricted variant of JavaScript, thereby implicitly opting-out of "sloppy mode".

* Strict mode eliminates some JavaScript silent errors by changing them to throw errors.
* Strict mode fixes mistakes that make it difficult for JavaScript engines to perform optimizations: strict mode code can sometimes be made to run faster than identical code that’s not strict mode.
* Strict mode prohibits some syntax likely to be defined in future versions of ECMAScript.
* It prevents, or throws errors, when relatively “unsafe” actions are taken (such as gaining access to the global object).
* It disables features that are confusing or poorly thought out.
* Strict mode makes it easier to write “secure” JavaScript.

[`^ Back to Top`](#contents)

## Types of Authentication:

* Cookie-Based authentication
* Token-Based authentication
* Third party access(OAuth, API-token)
* OpenId
* SAML

[`^ Back to Top`](#contents)

## 4 Patterns of Function Invocation
<table>
<tbody>
  <tr>
    <td colspan="1" rowspan="1">
      <p><span>Method Invocation</span></p>
    </td>
    <td colspan="1" rowspan="1">
      <p ><span >When a function is part of an object, it is called a method. Method invocation is the pattern of invoking a function that is part of an object.</span></p>
    </td>
  </tr>
  <tr>
    <td colspan="1" rowspan="1">
      <p><span>Function Invocation</span></p>
    </td>
    <td colspan="1" rowspan="1">
      <p ><span>When we call a function normally, we are using the function invocation pattern, and JavaScript will bind the value of this to the global object.</span></p>
    </td>
  </tr>
  <tr>
    <td colspan="1" rowspan="1">
      <p><span>Constructor Invocation</span></p>
    </td>
    <td colspan="1" rowspan="1">
      <p ><span class="c6">The constructor invocation pattern involves putting the new operator just before the function is invoked. </span><span>The this</span><span>&nbsp;parameter will be set to the newly created object and the return operator of the function will have its behavior altered.</span></p>
    </td>
  </tr>
  <tr>
    <td colspan="1" rowspan="1">
      <p><span>Apply And Call Invocation (and bind):</span></p>
    </td>
    <td colspan="1" rowspan="1">
      <p><span>The apply method allows manual invocation of a function. &nbsp;JavaScript also has another invoker called call, that is identical to apply except that instead of taking an array of parameters, it takes an argument list.</span></p>
    </td>
  </tr>
</tbody>
</table>

[`^ Back to Top`](#contents)

## 4 Principles of OOP
<table>
<tbody>
  <tr>
    <td colspan="1" rowspan="1">
      <p><span>Abstraction</span></p>
    </td>
    <td colspan="1" rowspan="1">
      <p><span>Abstract means a concept or an Idea which is not associated with any particular instance. Using abstract class/Interface we express the intent of the class rather than the actual implementation. In a way, one class should not know the inner details of another in order to use it, just knowing the interfaces should be good enough.</span></p>
    </td>
  </tr>
  <tr>
    <td colspan="1" rowspan="1">
      <p><span>Encapsulation </span></p>
    </td>
    <td colspan="1" rowspan="1">
      <p><span class="c2">Encapsulation is the mechanism of hiding of data
          implementation by restricting access to public methods. Instance variables are kept private and accessor methods are made public to achieve this.</span></p>
    </td>
  </tr>
  <tr>
    <td colspan="1" rowspan="1">
      <p><span>Inheritance </span></p>
    </td>
    <td colspan="1" rowspan="1">
      <p><span>Inheritances expresses “is-a” and/or “has-a” relationship between two objects. Using Inheritance, In derived classes we can reuse the code of existing super classes. In Java, concept of “is-a” is based on class inheritance (using extends) or interface implementation (using implements).</span></p>
    </td>
  </tr>
  <tr>
    <td colspan="1" rowspan="1">
      <p><span>Polymorphism </span></p>
    </td>
    <td colspan="1" rowspan="1">
      <p><span>Objects of classes belonging to the same hierarchical tree
          (inherited from a common base class) may possess functions bearing the same name, but
          each having different behaviors.</span></p>
    </td>
  </tr>
</tbody>
</table>

[`^ Back to Top`](#contents)

## Javascript Modules
<table>
<tbody>
  <tr>
    <td colspan="1" rowspan="1">
      <p><span>The Module pattern</span></p>
    </td>
    <tdcolspan="1" rowspan="1">
      <p><span class="c6">The Module Pattern is used to imitate the concept of classes, so we include methods and variables inside of a single object. That allows us to create a public facing API for the methods that we want to expose to the world, while still shielding private variables and methods in a closure scope and away from the global scope.
    </td>
  </tr>
  <tr>
    <td colspan="1" rowspan="1">
      <p><span>Object literal notation</span></p>
    </td>
    <td colspan="1" rowspan="1">
      <p><span>Encapsulation is the mechanism of hiding of data implementation by restricting access to public methods. Instance variables are kept private and accessor methods are made public to achieve this.</span></p>
    </td>
  </tr>
  <tr>
    <td colspan="1" rowspan="1">
      <p><span>AMD modules</span></p>
    </td>
    <td colspan="1" rowspan="1">
      <p><span>Asynchronous module definition is a specification for the programming language JavaScript. It defines an application programming interface that defines code module and their dependencies, and loads them asynchronously if desired.</span></p>
    </td>
  </tr>
  <tr>
    <td colspan="1" rowspan="1">
      <p><span">CommonJS modules</span></p>
    </td>
    <td colspan="1" rowspan="1">
      <p><span>The CommonJS module specification is the standard used in Node.js for working with modules. Modules are very cool, because they let you encapsulate all sorts of functionality, and expose this functionality to other JavaScript files, as libraries</span></p>
    </td>
  </tr>
  <tr>
    <td colspan="1" rowspan="1">
      <p><span>ECMAScript Harmony modules</span></p>
    </td>
    <td colspan="1" rowspan="1">
      <p><span>JavaScript modules are now supported by the browser. This means you can use this great addition in JavaScript, introduced by ECMAScript 2015, in the browser. Previously, you had to use a bundler such as a webpack in order to use modules. But no more. How cool is that!</span></p>
    </td>
  </tr>
</tbody>
</table>

[`^ Back to Top`](#contents)

## Types of Web Development Stacks
<table>
<tbody>
  <tr>
    <td colspan="1" rowspan="1">
      <p><span>LAMP </span></p>
    </td>
    <td colspan="1" rowspan="1">
      <p><span>(Linux, Apache, MySQL, PHP) – The Old-school Stack</span>
      </p>
    </td>
  </tr>
  <tr>
    <td colspan="1" rowspan="1">
      <p><spa>MEAN</span></p>
    </td>
    <td colspan="1" rowspan="1">
      <p><span>(MongoDB, ExpressJS, AngularJS, NodeJS) – The Jock Stack</span></p>
    </td>
  </tr>
  <tr>
    <td colspan="1" rowspan="1">
      <p><span>Meteor</span></p>
    </td>
    <td colspan="1" rowspan="1">
      <p><span>Written in JavaScript, Meteor is a beginner-friendly full-stack framework that can have an experienced programmer up and running in a few hours.</span></p>
    </td>
  </tr>
  <tr>
    <td colspan="1" rowspan="1">
      <p><span>MERN</span></p>
    </td>
    <td colspan="1" rowspan="1">
      <p><span>MERN consists of different open-source components: MongoDB, Express, React, and Node.js. All the components provide the end-to-end framework support for developers to work in.</span></p>
    </td>
  </tr>
</tbody>
</table>

[`^ Back to Top`](#contents)
