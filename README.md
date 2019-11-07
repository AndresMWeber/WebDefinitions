# WebDefinitions
A compendium of the web definitions and programming concepts I've come across in my time as a Web Deveoper

#### AUTHOR: Andres Weber

#### CONTRIBUTORS: 
- [Vitor Tomazzi](https://github.com/VitorTomazzi)

<hr style="page-break-before:always;display:none;">

JavaScript is not asynchronous language, but a synchronous one with some asynchronous behaviors. JavaScript, at its core, is a single-threaded and synchronous language.

<hr style="page-break-before:always;display:none;">

# Web Concepts and Acronyms
**WC3** - The World Wide Web Consortium (W3C) is an international community that develops open standards to ensure the long-term growth of the Web.
  
**TLD** - Top-level domain refers to the last segment of a domain name, or the part that follows immediately after the "dot" symbol.
  
**DOM** - The W3C Document Object Model (DOM) is a platform and language-neutral interface that allows programs and scripts to dynamically access and update the content, structure, and style of a document.
  
**BOM** - The Browser Object Model consists of the objects *navigator*, *history*, *screen*, *location* and *document* which are children of *window*.

**CRUD** - these operations are the four basic operations of persisting data (**C**reate, **R**ead, **U**pdate, **D**elete)
  
**AJAX** - short for asynchronous *JavaScript* and *XML*.  It is a set of web development techniques using many web technologies on the client side to create asynchronous web applications
  
**BSON** - Binary **JSON** (data format that **MongoDB** uses)
  
**ODM** -  Is an abstraction on top of our database connection: **ODMs** translate data from documents in our database, to objects in *JavaScript*.
  
**SSL** - **SSL** provides a secure channel between two machines or devices operating over the internet or an internal network.
  
**TLS** (**T**ransport **L**ayer **S**ecurity) is a protocol that provides authentication, privacy, and data integrity between two communicating computer applications. 
  
**HTTPS** (**H**ypertext **T**ransfer **P**rotocol **S**ecure) - is a variant of the standard web transfer protocol (HTTP) that adds a layer of security on the data in transit through a secure socket layer (**SSL**) or transport layer security (**TLS**) protocol connection.
  
**REST** (**RE**presentational **S**tate **T**ransfer) is an architectural style for developing web services. REST is popular due to its simplicity and the fact that it builds upon existing systems and features of the internet's Hypertext Transfer Protocol (**HTTP**) in order to achieve its objectives, as opposed to creating new standards, frameworks and technologies.
  
**RESTful** - A RESTful API -- also referred to as a RESTful web service -- is based on representational state transfer (**REST**) technology, an architectural style and approach to communications often used in web services development.

<hr style="page-break-before:always;display:none;">

**PAAS** (**P**latform **A**s **A** **S**ervice) - Is a cloud computing model in which a third-party provider delivers hardware and software tools -- usually those needed for application development -- to users over the internet. 
  
**IAAS** (**I**nfrastructure **A**s **A** **S**ervice) - Is a form of cloud computing that provides virtualized computing resources over the internet.

**SAAS** (**S**ubscription **A**s **A** **S**ervice) - A method of software delivery and licensing in which software is accessed online via a subscription, rather than bought and installed on individual computers.

**BDAAS** (**B**ig **D**ata **A**s **A** **S**ervice) - Is the delivery of statistical analysis tools or information by an outside provider that helps organizations understand and use the insights gained from large information sets in order to gain a competitive advantage.

**FAAS** (**Function** **A**s **A** **S**ervice) - Is a category of cloud computing services that provides a platform allowing customers to develop, run, and manage application functionalities without the complexity of building and maintaining the infrastructure typically associated with developing and launching an app.

**MAAS** (**Monitoring** **A**s **A** **S**ervice) - is a framework that facilitates the deployment of monitoring functionalities for various other services and applications within the cloud. The most common application for MaaS is online state monitoring, which continuously tracks certain states of applications, networks, systems, instances or any element that may be deployable within the cloud.

**NoSQL Database** - stands for "not only SQL," is an alternative to traditional relational databases in which data is placed in tables and data schema is carefully designed before the database is built.

**Non Relational Database** - A non-relational database is a database that does not use the tabular schema of rows and columns found in most traditional database systems. Instead, non-relational databases use a storage model that is optimized for the specific requirements of the type of data being stored.

**Intrinsic Web Design** - Content-driven design as opposed to design-driven.  CSS modules such as Flexbox allow developers to create layouts exactly as they want them to look, without the need for hacks and third-party frameworks. It gives  the flexibility to incorporate traditional layout techniques with modern ones based on a website’s intrinsic content.

**Static Web Applications** - sites that are delivered to a user's browser without any server-side processing.

**SOA** (**S**ervices **O**riented **A**rchitecture) aka **Microservices** - enables applications to communicate with each other on a single machine or when the applications are deployed on multiple machines across the network.

**Graceful Degradation** - the practice of building your web functionality so that it provides a certain level of user experience in more modern browsers, but it will also degrade gracefully to a lower level of user experience in older browsers.

**Progressive Enhancement** - starts by establishing a basic level of user experience that all browsers will be able to provide when rendering your web site, but you also build in more advanced functionality that will automatically be available to browsers that can use it.

**Doctype** - doctypes were meant to act as links to a set of rules that the HTML page had to follow to be considered good HTML, which could mean automatic error checking and other useful things.

**FOUC** (**F**lash **O**f **U**nstyled **C**ontent) - when a stylesheet loads in a delayed manner and the html content is unstyled until it loads.

**ARIA** (**A**ssistive **R**ich **I**nternet **A**pplications) -  is a spec from the World Wide Web Consortium (W3C) that was created to improve accessibility of web pages and applications by providing extra information to screen readers via HTML attributes.

**SEO** (**S**earch **E**ngine **O**ptimization) is the process of increasing the quality and quantity of website traffic by increasing the visibility of a website or a web page to users of a web search engine.

**BFC** (Block Formatting Context) - A block formatting context is a part of a visual CSS rendering of a Web page. It is the region in which the layout of block boxes occurs and in which floats interact with each other. Floats, absolutely positioned elements, inline-blocks, table-cells, table-captions, and elements with overflow other than visible (except when that value has been propagated to the viewport) establish new block formatting contexts.

**Resetting CSS** - Resetting is meant to strip all default browser styling on elements. For e.g. margins, paddings, font-sizes of all elements are reset to be the same. You will have to redeclare styling for common typographic elements.

**Normalizing CSS** - Normalizing preserves useful default styles rather than “unstyling” everything. It also corrects bugs for common browser dependencies.

**CORS** (**C**ross-**O**rigin **R**esource **S**haring) - is a mechanism that uses additional HTTP headers to tell browsers to give a web application running at one origin, access to selected resources from different origins.


# Services

**MongoDB** (DBAAS) - MongoDB is a non-relational database that stores data in collections. It stores data in flexible, JSON-like, meaning fields can vary from document to document and over the time the data structure can change.

**Redux** - Redux is a predictable state container library for JavaScript apps.  It helps you write applications that behave consistently, run in different environments (client, server, and native), and are easy to test.

**redux-thunk** - middleware to help us make requests in a Redux application

**react-redux** - Integration layer between React and Redux

**Redis** - Redis is an open source (BSD licensed), in-memory data structure store, used as a database, cache and message broker. It supports data structures such as strings, hashes, lists, sets, sorted sets with range queries, bitmaps, hyperloglogs, geospatial indexes with radius queries and streams. Redis has built-in replication, Lua scripting, LRU eviction, transactions and different levels of on-disk persistence, and provides high availability via Redis Sentinel and automatic partitioning with Redis Cluster.

**AWS** - Amazon Web Services Whether you're looking for compute power, database storage, content delivery, or other functionality, AWS has the services to help you build sophisticated applications with increased flexibility, scalability and reliability

**AWS Elastic Beanstalk** (PAAS) -Is an orchestration service offered by Amazon Web Services for deploying applications which orchestrates various AWS services, including EC2, S3, Simple Notification Service, CloudWatch, autoscaling, and Elastic Load Balancers.

**AWS LAMBDA** (FAAS) - Is grouped under "Serverless / Task Processing" or FAAS (Functions As A Service)

**AWS EC2** - Amazon Elastic Compute Cloud (Amazon EC2) is a web service that provides secure, resizable compute capacity in the cloud. It is designed to make web-scale cloud computing easier for developers.

**AWS EMR** (BDAAS) - Amazon EMR can be classified as a tool in the "Big Data as a Service"

**Kubernetes** (k8s) - is an open-source container-orchestration system for automating application deployment, scaling, and management.

**Heroku** (PAAS) - Heroku is a cloud platform that lets companies build, deliver, monitor and scale apps.

**Microsoft Azure** (PAAS) -

**BitNami** (PAAS) -

**Cloudways** (PAAS) -

**IBM Cloud Platform** (ICP) (Bluemix) (PAAS) - IBMs’ PaaS offering was known as ‘IBM Bluemix’ earlier, however, IBM now offers it as the overall IBM Cloud Platform. IBM Cloud Platform offers you a range of choices for running your app, for e.g.: As a Cloud Foundry app, As a Docker container on a Kubernetes cluster, As VMware, As a virtual machine.

**Salesforce Platform** (APAAS) - Salesforce aPaaS uses Heroku for deploying, running, and managing apps. Their ‘Lightning Design’ system offers guides and sample codes for developers, who can then get started with the app development quickly.

**Jelastic** (PAAS) -

**Oracle Cloud Platform** (OCP) (PAAS) -

**Google Anthos or Google App Engine** (GAE) (PAAS) -

**Red Hat Openshift** (PAAS) -  Red Hat OpenShift PaaS takes advantage of the reliability and security that Red Hat Enterprise Linux offers. It combines that with the OpenStack IaaS. On top of that, you can build your apps with Red Hat JBoss Enterprise Application Platform (EAP). This should allow you to focus on your code without unnecessary diversion of infrastructure and runtime environment-related concerns!

**Stackify** (MAAS) -

**DataDog** (MAAS) -

# Programming Terms/Concepts

**Primitive** - A primitive (primitive value, primitive data type) is data that is not an object and has no methods. In JavaScript, there are 6 primitive data types: string, number, boolean, null, undefined, symbol (new in ECMAScript 2015).

**Function Expression** - Storing an anonymous function in a variable.

**Function Statement** (Function Literals) - Traditional function definition with the function keyword.

**Callback Function** - A callback is a function that is to be executed after another function has finished executing — hence the name ‘call back’.

**Shadowing** - In computer programming, variable shadowing occurs when a variable declared within a certain scope has the same name as a variable declared in an outer scope:

**Closure** - A closure is the combination of a function and the lexical environment within which that function was declared.  Sometimes represented as an expression (usually a function) that can have free variables together with an environment that binds those variables (it “closes” the expression).

**Static Properties** - properties of a class, or dot notation accessible variables stored at the class level and not on the instance level.

**Black Box Programming** - Programming in a black-box paradigm mainly consists of having functions or methods that hides the inner workings from the user (programmer). These functions take a set number of parameters and produce the given output without the developer having to worry about how the actual logic is implemented.

**Block Scope** - Lexical scope that is contained between two curly braces.

**Function Scope** - Lexical scope that is contained within a function.

**Lexical Scoping** - is a convention used with many programming languages that sets the scope (range of functionality) of a variable so that it may only be called (referenced) from within the block of code in which it is defined.

* Suspends execution of the current function
* Passes controls to the invoked function
* Passes (secretly) two parameters to the invoked function:
  * An array named arguments
  * A parameter named this

**Scaffolding** - Scaffolding, as used in computing, refers to one of two techniques: The first is a code generation technique related to database access in some model–view–controller frameworks; the second is a project generation technique supported by various tools.

**Bootstrapping** - An example of bootstrapping is in some web frameworks. You call index.php (the bootstrapper), and then it loads the frameworks helpers, models, configuration, and then loads the controller and passes off control to it.

**Tree Shaking** - Tree shaking means removing “dead code” from the bundle you ship to your users. If you add some code that you never use in your import statements, that’s not going to be sent to the users of your app, to reduce file size and loading time.

**Transpilation** - Transpilers, or source-to-source compilers, are tools that read source code written in one programming language, and produce the equivalent code in another language.

**Boilerplate** - A boilerplate is a unit of writing that can be reused over and over without change. By extension, the idea is sometimes applied to reusable programming, as in “boilerplate code.”

**Curried (*Currying a*) Function** - Currying is a process in functional programming in which we can transform a function with multiple arguments into a sequence of nested functions. It returns a new function that expects the next argument inline.

**Higher Order (*x*)** - Higher-order programming is a style of computer programming that uses software components, like functions, modules or objects, as values. It is usually instantiated with, or borrowed from, models of computation such as lambda calculus which makes heavy use of higher-order functions.  Functions that operate on other functions, either by taking them as arguments or by returning them, are called higher-order functions.

**First Class Citizen** - is an entity which supports all the operations generally available to other entities. These operations typically include being passed as an argument, returned from a function, modified, and assigned to a variable. (e.g. functions are first class citizens in JavaScript)

**Prototype Delegation** - herein an object will search its entire prototype chain for a given property (for example, a Chicken object delegating a layEgg behavior to a higher-up prototype Bird object.)

**Object Linked to Other Object (OLOO) Pattern** - In this pattern, we don’t use a function to create objects at all. Instead, we define a blueprint object of sorts, which we then explicitly use as the prototype for any individual objects we need. In JavaScript this is implemented like so: ```Object.create(myObj)```  OLOO allows us to share like behaviors and check the type of individual objects, all while sidestepping the class illusions inherent in the constructor and pseudo-classical patterns.

## Prototypal Inheritance vs Classical Inheritance
**Framework** - A universal, reusable software environment to facilitate the development of software applications, products and solutions.

* It describes the structure of the application.
* It gives the developer a way to organize the code to make an app more flexible and scalable.

**Library**  -
* one library can be combined with multiple other libraries, while that’s not the case with frameworks - it’s almost impossible to have two frameworks combined on the same app
* set of functions/methods/events that developers can use in order to achieve wanted behavior of the app
* using a library gives more freedom to developers but that also means more responsibility for the design of the whole system and app flow and it carries more risk as well.

**Imperative Programming** -  imperative programming is a programming paradigm that uses statements that change a program's state. In much the same way that the imperative mood in natural languages expresses commands, an imperative program consists of commands for the computer to perform. Imperative programming focuses on describing how a program operates.

**Declarative Programming** - declarative programming is a programming paradigm — a style of building the structure and elements of computer programs—that expresses the logic of a computation without describing its control flow.

**MVC Pattern** -  To solve this problem, we can use the pattern **MVC** (**M**odel-**V**iew-**C**ontroller) that adds the ```Model``` in such a way that:

* Every time a **Request** is made on the server, a Controller handles it.
* This **Controller** will communicate with Models.
Models will read and write data directly to a database.
* When the **Controller** has all information, it can pass that data to the **View**.
* The **View** generates a **Response** which is a **HTML** page rendered to a client (in a browser).

**Programming Paradigm** - A programming paradigm is a fundamental style of building the structure and elements of a program. The styles and capabilities of programming languages are defined by their paradigms.


## Common Programming Paradigms
* **Imperative**: Programming with an explicit sequence of commands that update state.
* **Declarative**: Programming by specifying the result you want, not how to get it.
* **Structured**: Programming with clean, goto-free, nested control structures.
* **Procedural**: Imperative programming with procedure calls.
* **Functional** (Applicative): Programming with function calls that avoid any global state.
* **Function-Level** (Combinator): Programming with no variables at all.
* **Object-Oriented**: Programming by defining objects that send messages to each other. Objects have their own internal (encapsulated) state and public interfaces. Object orientation can be:
* **Class-based**: Objects get state and behavior based on membership in a class.
* **Prototype-based**: Objects get behavior from a prototype object.
* **Event-Driven**: Programming with emitters and listeners of asynchronous actions.
* **Flow-Driven**: Programming processes communicating with each other over predefined channels.
* **Logic** (Rule-based): Programming by specifying a set of facts and rules. An engine infers the answers to questions.
* **Constraint**: Programming by specifying a set of constraints. An engine finds the values that meet the constraints.
* **Aspect-Oriented**: Programming cross-cutting concerns applied transparently.
* **Reflective**: Programming by manipulating the program elements themselves.
* **Array**: Programming with powerful array operators that usually make loops unnecessary.

**Design Pattern** - a design pattern is a tried and tested solution to a common programming pattern. It could be considered a best practice. If you approach a program using an Object Oriented paradigm, there are a number of design patterns you can then draw on to solve specific problems.

# Design Pattern Classifications

**Creational Design Patterns** - These design patterns are all about class instantiation. This pattern can be further divided into class-creation patterns and object-creational patterns. While class-creation patterns use inheritance effectively in the instantiation process, object-creation patterns use delegation effectively to get the job done.

**Structural Design Patterns** - These design patterns are all about Class and Object composition. Structural class-creation patterns use inheritance to compose interfaces. Structural object-patterns define ways to compose objects to obtain new functionality.

**Behavioral Design Patterns** - These design patterns are all about Class's objects communication. Behavioral patterns are those patterns that are most specifically concerned with communication between objects.


# Common Design Patterns
**Singleton** - Only one instance of the given class may exist at any time.

**Strategy** - A local strategy will change based on a given situation.

**Factory** - You can create many different objects from one Factory based on criteria without the need to directly instantiate the class.

**Builder** - Splits up the construction of an object from the representation almost like an interface to the object so that we can customize the representation of that object.

**Chain of Responsibility** - A stack type implementation that checks the objects as it goes for validity in order to continue, often used as a failsafe.

**Template** - create a “template” for high order operations/order usually as an abstract class and then the class that extends that will fill in the details with helper functions or implementing those sub-functions of the high order operation.

**State** - Allows behavior of the class to change based on the current state of the object.

# JavaScript Terms/Concepts
**Immediately-invoked function expression** (**IIFE**) -  is a JavaScript design pattern which produces a lexical scope using JavaScript’s function scoping.

* avoid variable hoisting from within blocks
* protect against polluting the global environment and
* simultaneously allow public access to methods while retaining privacy for variables defined within the function

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

**Rest Pattern (ES6)** - allows you to spread as many components of a container into variables and catch the “rest” of the container’s components you did not specify variables for.

**Spread (ES6)** - allows you to expand something that is currently grouped inside a particular container and assign it to a different container

**for/in Loop (ES 1st Edition)** - When using for/in loops with arrays, it is important to note that the “key” of an array is just the index. So when using a for/in loop with an array you will not get the value at each index, instead, you will get the index.

**for/of Loop (ES6)** - a recent addition that is specifically intended to iterate over iterable objects, like arrays, strings, maps, and sets. Syntactically, it is almost identical to the for/in loop except you replace in with of. Functionally they are different. Instead of getting the key, like the for/in loop, you get the actual value at that location.

**Destructuring Assignment** - Taking an array/object and splitting its component indices and storing into receiving variables.

```const [first, second, ...rest] = ['some', 'long', 'array', 'of', 'values']```

**Anonymous closure** - these functions have its own evaluation environment or “closure”, and then we immediately evaluate it. This lets us hide variables from the parent (global) namespace.

**Module pattern** - was used to mimic the concept of classes (since JavaScript doesn’t natively support classes) so that we can store both public and private methods and variables inside a single object.

**Hoisting** - Hoisting is JavaScript's default behavior of moving all declarations to the top of the current scope (to the top of the current script or the current function).  JavaScript only hoists declarations, not initializations.

**Promise (ES2015)** - A Promise is an object representing the eventual completion or failure of an asynchronous operation. Essentially, a promise is a returned object to which you attach callbacks, instead of passing callbacks into a function.

**Arrow Function (ES6)** - These are anonymous functions with their own special syntax that accept a fixed number of arguments, and operate in the context of their enclosing scope — ie the function or other code where they are defined.

**Node Require vs Import (ES2015)** - Require can be called within a scope, but import can only be called in the global scope, therefore reducing a lot of pressure on transpilers that cannot introspect/tree shake properly in that situation.

**Polyfill** - In web development, a polyfill is code that implements a feature on web browsers that do not support the feature. Most often, it refers to a JavaScript library that implements an HTML5 web standard, either an established standard (supported by some browsers) on older browsers, or a proposed standard (not supported by any browsers) on existing browsers. Formally, "a polyfill is a shim for a browser API"

**Strict Mode** - JavaScript's strict mode, introduced in ECMAScript 5, is a way to opt in to a restricted variant of JavaScript, thereby implicitly opting-out of "sloppy mode".

* Strict mode eliminates some JavaScript silent errors by changing them to throw errors.
* Strict mode fixes mistakes that make it difficult for JavaScript engines to perform optimizations: strict mode code can sometimes be made to run faster than identical code that’s not strict mode.
* Strict mode prohibits some syntax likely to be defined in future versions of ECMAScript.
* It prevents, or throws errors, when relatively “unsafe” actions are taken (such as gaining access to the global object).
* It disables features that are confusing or poorly thought out.
* Strict mode makes it easier to write “secure” JavaScript.

#### Types of Authentication:

* Cookie-Based authentication
* Token-Based authentication
* Third party access(OAuth, API-token)
* OpenId
* SAML


<table>
<tbody>
  <tr>
    <td colspan="2" rowspan="1">
      <h3><span>4 Patterns of Function Invocation</span></h3>
    </td>
  </tr>
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



<table class="c48">
<tbody>
  <tr class="c46">
    <td class="c59" colspan="2" rowspan="1">
      <h3 class="c10" id="h.viek25iet3ul"><span class="c50 c47 c7">4 Principles of OOP</span></h3>
    </td>
  </tr>
  <tr class="c32">
    <td class="c23" colspan="1" rowspan="1">
      <p class="c42 c40"><span class="c1">Abstraction</span></p>
    </td>
    <td class="c68" colspan="1" rowspan="1">
      <p class="c42 c40"><span class="c2">Abstract means a concept or an Idea which is not associated with any particular instance. Using abstract class/Interface we express the intent of the class rather than the actual implementation. In a way, one class should not know the inner details of another in order to use it, just knowing the interfaces should be good enough.</span></p>
    </td>
  </tr>
  <tr class="c46">
    <td class="c23" colspan="1" rowspan="1">
      <p class="c42 c40"><span class="c1">Encapsulation </span></p>
    </td>
    <td class="c68" colspan="1" rowspan="1">
      <p class="c42 c40"><span class="c2">Encapsulation is the mechanism of hiding of data
          implementation by restricting access to public methods. Instance variables are kept private and accessor methods are made public to achieve this.</span></p>
    </td>
  </tr>
  <tr class="c46">
    <td class="c23" colspan="1" rowspan="1">
      <p class="c42 c40"><span class="c1">Inheritance </span></p>
    </td>
    <td class="c68" colspan="1" rowspan="1">
      <p class="c42 c40"><span class="c2">Inheritances expresses “is-a” and/or “has-a” relationship between two objects. Using Inheritance, In derived classes we can reuse the code of existing super classes. In Java, concept of “is-a” is based on class inheritance (using extends) or interface implementation (using implements).</span></p>
    </td>
  </tr>
  <tr class="c46">
    <td class="c23" colspan="1" rowspan="1">
      <p class="c42 c40"><span class="c1">Polymorphism </span></p>
    </td>
    <td class="c68" colspan="1" rowspan="1">
      <p class="c42 c40"><span class="c2">Objects of classes belonging to the same hierarchical tree
          (inherited from a common base class) may possess functions bearing the same name, but
          each having different behaviors.</span></p>
    </td>
  </tr>
</tbody>
</table>



<table class="c48">
<tbody>
  <tr class="c90">
    <td class="c67" colspan="2" rowspan="1">
      <h3 class="c10" id="h.zguowv5mlvaf"><span>Javascript </span><span
          class="c50 c47 c7">Modules</span></h3>
    </td>
  </tr>
  <tr class="c46">
    <td class="c22" colspan="1" rowspan="1">
      <p class="c42 c40"><span class="c1">The Module pattern</span></p>
    </td>
    <td class="c61" colspan="1" rowspan="1">
      <p class="c42 c40"><span class="c6">The Module Pattern is used to imitate the concept of classes, so we include methods and variables inside of a single object. That allows us to create a public facing API for the methods that we want to expose to the world, while still shielding private variables and methods in a closure scope and away from the global scope.
    </td>
  </tr>
  <tr class="c46">
    <td class="c22" colspan="1" rowspan="1">
      <p class="c42 c40"><span class="c1">Object literal notation</span></p>
    </td>
    <td class="c61" colspan="1" rowspan="1">
      <p class="c42 c40"><span class="c2">Encapsulation is the mechanism of hiding of data implementation by restricting access to public methods. Instance variables are kept private and accessor methods are made public to achieve this.</span></p>
    </td>
  </tr>
  <tr class="c46">
    <td class="c22" colspan="1" rowspan="1">
      <p class="c42 c40"><span class="c1">AMD modules</span></p>
    </td>
    <td class="c61" colspan="1" rowspan="1">
      <p class="c42 c40"><span class="c2">Asynchronous module definition is a specification for the programming language JavaScript. It defines an application programming interface that defines code module and their dependencies, and loads them asynchronously if desired.</span></p>
    </td>
  </tr>
  <tr class="c46">
    <td class="c22" colspan="1" rowspan="1">
      <p class="c42 c40"><span class="c60 c1">CommonJS modules</span></p>
    </td>
    <td class="c61" colspan="1" rowspan="1">
      <p class="c42 c40"><span class="c2">The CommonJS module specification is the standard used in Node.js for working with modules. Modules are very cool, because they let you encapsulate all sorts of functionality, and expose this functionality to other JavaScript files, as libraries</span></p>
    </td>
  </tr>
  <tr class="c90">
    <td class="c22" colspan="1" rowspan="1">
      <p class="c42 c41"><span class="c60 c1">ECMAScript Harmony modules</span></p>
    </td>
    <td class="c61" colspan="1" rowspan="1">
      <p class="c42"><span class="c2">JavaScript modules are now supported by the browser. This means you can use this great addition in JavaScript, introduced by ECMAScript 2015, in the browser. Previously, you had to use a bundler such as a webpack in order to use modules. But no more. How cool is that!</span></p>
    </td>
  </tr>
</tbody>
</table>




<table>
<tbody>
  <tr>
    <td colspan="2" rowspan="1">
      <h3><span>Types of Web Development Stacks</span></h3>
    </td>
  </tr>
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
    <td class="c23" colspan="1" rowspan="1">
      <p class="c42 c40"><span class="c1">MEAN </span></p>
    </td>
    <td class="c27" colspan="1" rowspan="1">
      <p class="c42 c40"><span class="c2">&nbsp;(MongoDB, ExpressJS, AngularJS, NodeJS) &nbsp;– The
          Jock Stack</span></p>
    </td>
  </tr>
  <tr class="c46">
    <td class="c23" colspan="1" rowspan="1">
      <p class="c42 c40"><span class="c1">Meteor</span></p>
    </td>
    <td class="c27" colspan="1" rowspan="1">
      <p class="c42 c40"><span class="c2">Written in JavaScript, Meteor is a beginner-friendly
          full-stack framework that can have an experienced programmer up and running in a few
          hours.</span></p>
    </td>
  </tr>
  <tr class="c46">
    <td class="c23" colspan="1" rowspan="1">
      <p class="c40 c42"><span class="c1">MERN</span></p>
    </td>
    <td class="c27" colspan="1" rowspan="1">
      <p class="c42 c40"><span class="c2">MERN consists of different open-source components: MongoDB,
          Express, React, and Node.js. All the components provide the end-to-end framework support
          for developers to work in.</span></p>
    </td>
  </tr>
</tbody>
</table>



<table>
<tbody>
  <tr>
    <td colspan="2" rowspan="1">
      <h3><span>Types of Databases</span></h3>
    </td>
  </tr>
  <tr>
    <td colspan="1" rowspan="1">
      <p><span>SQL / RDBMS / Relational databases</span></p>
    </td>
    <td colspan="1" rowspan="1">
      <p><span><a
            href="https://www.google.com/url?q=https://www.oracle.com/index.html&amp;sa=D&amp;ust=1572995788433000">Oracle</a></span><span
          class="c6">, </span><span class="c29 c6"><a class="c21"
            href="https://www.google.com/url?q=https://www.mysql.com/&amp;sa=D&amp;ust=1572995788433000">MySQL</a></span><span
          class="c6">, </span><span class="c29 c6"><a class="c21"
            href="https://www.google.com/url?q=https://www.microsoft.com/en-us/sql-server/default.aspx&amp;sa=D&amp;ust=1572995788433000">Microsoft
            SQL Server</a></span><span class="c6">, </span><span class="c29 c6"><a class="c21"
            href="https://www.google.com/url?q=https://www.postgresql.org/&amp;sa=D&amp;ust=1572995788433000">PostgreSQL</a></span><span
          class="c6">, </span><span class="c29 c6"><a class="c21"
            href="https://www.google.com/url?q=https://www.ibm.com/analytics/db2&amp;sa=D&amp;ust=1572995788434000">DB2</a></span>
      </p>
    </td>
  </tr>
  <tr>
    <td colspan="1" rowspan="1">
      <p><span>NoSQL / Non-relational databases</span></p>
      <p><span></span></p>
      <p><span></span></p>
    </td>
    <td colspan="1" rowspan="1">
      <p><span>Key-Value Stores: </span><span><a
            href="https://www.google.com/url?q=https://redis.io/&amp;sa=D&amp;ust=1572995788435000">Redis
          </a></span><span>and</span><span><a
            href="https://www.google.com/url?q=https://aws.amazon.com/dynamodb/&amp;sa=D&amp;ust=1572995788435000">&nbsp;Amazon
            DynamoDB</a></span></p>
      <p><span>Wide Column Stores:</span><span>&nbsp;</span><span><a 
            href="https://www.google.com/url?q=http://cassandra.apache.org/&amp;sa=D&amp;ust=1572995788436000">Cassandra</a></span><span>, </span><span><a
            href="https://www.google.com/url?q=https://www.scylladb.com/&amp;sa=D&amp;ust=1572995788436000">Scylla</a></span><span>, and </span><span><a 
            href="https://www.google.com/url?q=https://hbase.apache.org/&amp;sa=D&amp;ust=1572995788436000">HBase</a></span>
      </p>
      <p><span>Document Stores: </span><span"><a
            href="https://www.google.com/url?q=https://www.mongodb.com/&amp;sa=D&amp;ust=1572995788437000">MongoDB</a></span"><span>&nbsp;and </span><span><a
            href="https://www.google.com/url?q=https://www.couchbase.com/&amp;sa=D&amp;ust=1572995788437000">Couchbase</a></span>
      </p>
      <p><span>Graph Databases: </span><span><a
            href="https://www.google.com/url?q=https://neo4j.com/lp/try-neo4j-sandbox/?ref%3Dplp%26utm_source%3Dgoogle%26utm_medium%3Dppc%26utm_campaign%3D*NA%2520-%2520Search%2520-%2520Branded%26utm_adgroup%3D*NA%2520-%2520Search%2520-%2520Branded%2520-%2520Neo4j%2520-%2520Exact%26utm_term%3Dneo4j%26gclid%3DCj0KCQjwoebsBRCHARIsAC3JP0Lwu4Fq-kzLzgYxDV9070xi7GIClh6rw83Vwzlz_T6LZpj3uPdzxxkaAs6zEALw_wcB&amp;sa=D&amp;ust=1572995788437000">Neo4J
          </a></span><span>and </span><span><a
            href="https://www.google.com/url?q=https://www.datastax.com/&amp;sa=D&amp;ust=1572995788438000">Datastax</a></span>
      </p>
      <p><span>Search Engines:</span><span>&nbsp;</span><span><a 
            href="https://www.google.com/url?q=https://www.elastic.co/&amp;sa=D&amp;ust=1572995788438000">Elasticsearch</a></span><span>, </span><span><a
            href="https://www.google.com/url?q=https://www.splunk.com/&amp;sa=D&amp;ust=1572995788438000">Splunk</a></span><span>, </span><span><a
            href="https://www.google.com/url?q=https://lucene.apache.org/solr/&amp;sa=D&amp;ust=1572995788438000">Solr</a></span>
      </p>
      <p><span>H</span><span>ybrid Row/Column Store: </span><span><a href="https://www.google.com/url?q=https://ai.google/research/pubs/pub27898&amp;sa=D&amp;ust=1572995788439000">Bigtable</a></span>
      </p>
    </td>
  </tr>
</tbody>
</table>

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

# Redux

## Redux Workflow
  * **Action Creator** - Changes the state of the app: produces an object.
  * **Action** - The action object that will run after action has been created from template Action Creator.
  * **Dispatch** - Receives any action and feeds to reducers.
  * **Reducers** - Process forms/data that comes in, modify and return processed data
  * **State** - Receives reducer data that gets added to a state object which waits until new actions to update next.

## React-Redux
  * **Provider** - takes in the redux store/state as a prop at the top level around the App.
  * **Connect** - registers action creators and hooks them up with the Provider at the top level via the context system to allow the actions to affect the state.  Connect also is able to hook up Components with the prodiver’s redux state and also remap any redux state values to different prop names.

**Async/Sync Action Creators** - disallowed in redux actions: this is due to post-transpilation code returning a request object, not the plain object we are expecting.  You need middleware!

**Redux Thunk** - Middleware solution for asynchronous action creators to allow pausing of actions (enforcing synchronicity) between dispatch/reducer cycle and remove race conditions.

## Rules of Reducers

  1. Must return any value besides ‘undefined’
  1. Produces ‘state’, or data to be used inside of your app using only previous state and the action (reducers are pure) (NO API REQUESTS, USER INPUT OR DOM QUERYING etc)
  1. Must not reach ‘out of itself’ to decide what value to return
  1. Must not mutate its input ‘state’ argument

# The Front End
**SEO** - **S**earch **E**ngine **O**ptimization

**CSS** - **C**ascading **S**tyle **S**heets

**SASS** - **S**yntactically **A**wesome **S**tyle **S**heets, is a preprocessor scripting language that is interpreted or compiled into *CSS*.

**SCSS** - Sassy CSS is a newer syntax for *SASS*. The formatting is similar to *CSS* with curly braces and semicolons. While the original syntax for *SASS* was more like *Python* with no curly braces and semicolons and heavy emphasis on tabbing.

**DNS** (**D**omain **N**ame **S**ervice) - when you register a domain, you can set many types of *DNS* Records.  Each record has a *Type*, a *Host*, and a *Value*

  1. **"Types"** are predefined
  1. **"Host"** represents the root (**@**) or a subdomain (**www**)
  1. **"Value"** is an IP or web address, or other value

## DNS Types:
**CNAME** - maps a subdomain to another domain name.  This can be another subdomain on the same site (like forwarding www to the root (**@**)).  Once you define a *CNAME* record for a subdomain (host), you *CAN'T DEFINE* another record for that same subdomain.  Because of this, you can't use *CNAME* at the root level (where you need other records to exist).  **CANNOT USE THIS ON THE ROOT (@)**

Ex: ```www.example.com => example.com```

**A/AAAA** - maps a subdomain to an *IPv4* address. This is most commonly used at the root, so it tells your browser where ```example.com``` lives.  **CAN DO THIS ON THE ROOT (@)**. If your domain does not have a static IP you cannot use A record.

Ex: ```example.com => 127.0.0.1```

Ex: ```example.com => ::1```

**ALIAS/ANAME/Virtual CNAME**- *ALIAS* is like *CNAME*, but it's a non-standard dns type.  So you can use *ALIAS* to forward your root domain (```example.com```) to your app's server (```example.herokudns.com```)

Ex: ```example.com => example.netlify.com```

**TXT** - *TXT* records, which provide extra info to any computer reading the *DNS* record.  *TXT* records are often used to prove you own a domain - because only the domain owner can set a *DNS* record.

Ex: ```@ => my-domain-is-awesome-123```