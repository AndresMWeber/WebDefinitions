
# Programming Terms/Concepts

# Contents
[`Contents`](#contents)

[`Definitions`](#definitions)

[`Prototypal Inheritance vs Classical Inheritance`](#prototypal-inheritance-vs-classical-inheritance)

[`Common Programming Paradigms`](#common-programming-paradigms)

[`Design Pattern Classifications`](#design-pattern-classifications)

[`Common Design Patterns`](#common-design-patterns)

## Definitions

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

[`^ Back to Top`](#contents)

## Prototypal Inheritance vs Classical Inheritance
<p align="center">
    <img src=https://raw.githubusercontent.com/AndresMWeber/WebDefinitions/master/media/7_Inheritance.png>
</p>

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

[`^ Back to Top`](#contents)

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

[`^ Back to Top`](#contents)

# Design Pattern Classifications

**Creational Design Patterns** - These design patterns are all about class instantiation. This pattern can be further divided into class-creation patterns and object-creational patterns. While class-creation patterns use inheritance effectively in the instantiation process, object-creation patterns use delegation effectively to get the job done.

**Structural Design Patterns** - These design patterns are all about Class and Object composition. Structural class-creation patterns use inheritance to compose interfaces. Structural object-patterns define ways to compose objects to obtain new functionality.

**Behavioral Design Patterns** - These design patterns are all about Class's objects communication. Behavioral patterns are those patterns that are most specifically concerned with communication between objects.

[`^ Back to Top`](#contents)

# Common Design Patterns
**Singleton** - Only one instance of the given class may exist at any time.

**Strategy** - A local strategy will change based on a given situation.

**Factory** - You can create many different objects from one Factory based on criteria without the need to directly instantiate the class.

**Builder** - Splits up the construction of an object from the representation almost like an interface to the object so that we can customize the representation of that object.

**Chain of Responsibility** - A stack type implementation that checks the objects as it goes for validity in order to continue, often used as a failsafe.

**Template** - create a “template” for high order operations/order usually as an abstract class and then the class that extends that will fill in the details with helper functions or implementing those sub-functions of the high order operation.

**State** - Allows behavior of the class to change based on the current state of the object.

[`^ Back to Top`](#contents)