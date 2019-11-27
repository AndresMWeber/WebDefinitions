


<h1 align="center">ANGULAR</h1>
<p align="center">
    <img width="200px" src=https://raw.githubusercontent.com/AndresMWeber/WebDefinitions/master/media/Angular.png>
</p>

# Contents
[`Components`](#components)

[`Component Lifecycle Methods`](#component-lifecycle-methods)

[`Databinding`](#databinding)

[`Directives`](#directives)

[`Templates`](#templates)

[`Services`](#services)

[`Dependency Injection`](#dependency-injection)

[`Routing`](#routing)

[`Observables`](#observables)

[`Forms`](#forms)

[`Pipes`](#pipes)

## Components
Angular uses a **decorator** in order to wrap whatever class you create as a component.  This contrasts with **React's** ```extend``` style class definition.  You pass an ```object``` that has an optional ```selector``` and a ```templateUrl``` or ```template``` field that specifies the html file that contains its skeleton.  

Angular also has a CLI tool that allows you to generate the scaffolding for any given component using ```ng generate component``` among many other features.

| key    | description | 
| :----- | :-----  |
| selector  | The HTML element that you refer to in order to instantiate this Angular Component|
| templateUrl  | Path to an HTML template file that will determine the Component's DOM representation |
| template  | Hard coded HTML template instead of using a file |
| encapsulation | Override for the default Shadow DOM encapsulation of the Component |

- **Cross-Component Communication** - Using ```@Input``` (similar to React props) and ```@Output``` (similar to Redux global state) decorators to allow **Angular Component** properties to be available as cross component bindable properties and custom events using ```@Output propertName = new EventEmitter<eventData>()```.

[`^ Back to Top`](#contents)

## Component Lifecycle Methods

To allow your Component to make use of the lifecycle methods you must add them in the class definition and import them from ```@angular/core```.  
E.g: ```export class MyComponent implements OnInit, OnChanges```

| Name (import from @angular/core just remove the ng) | Description |
| :----- | :----- |
| ```ngOnChanges```  | Called after a bound input property changes, receives one argument that represents the changes to be made with each key having an object with the structure ```{currentValue: value, firstChange: boolean, previousValue: value}```. |
| ```ngOnInit``` | Called once the component is initialized |
| ```ngDoCheck``` | Called during every change detection run |
| ```ngAfterContentInit``` | Called every time the projected content has been checked |
| ```ngAfterViewInit``` | Called after the component's view (and child views) have been initialized |
| ```ngAfterViewChecked``` | Called every time the view (and child views) have been checked |
| ```ngOnDestroy``` | Called once the component is about to be destroyed |

[`^ Back to Top`](#contents)

## Databinding
* **String Manipulation** - ```{{propertyName}}```

* **Property Binding** - ```[htmlProperty ]="angularClassProperty"``` - Derives the value of the angular class instance property that you set the html element's property equal to.

* **Event Binding** - ```(eventName)="angularClassMethod()"``` - Allows to bind a DOM element's event to the Angular class instance method.

* **Two-Way Databinding** - ```([ngModel])="angularClassPropertyToBind``` - Allows two way bound class properties that can be set from the html element or from the angular class instance property.

* **Custom Property Binding** - (in Angular view component class definition) ```@Input('customPropertyAlias') property``` - Now you can bind to this property anywhere in the angular html view files.  To add an alias to these properties, just pass a string in the Input decorator as a string (not recommended unless necessary).

[`^ Back to Top`](#contents)

## Directives
Directives are a class like a component but without a view or template that modify their host elements based on new abilities provided by the directives.
* ```*ngIf="conditionalExpression" (#elseCondition)``` - Structural Directive that allows conditional DOM manipulation.
* ```*ngFor=let element of iterable; let i = index``` - Structural Directive that allows iterable DOM manipulation.
* ```[ngStyle]=``` - Attribute Directive dynamically modifies the appearance/styling of an element.
* ```[ngClass]={className: boolean expression}``` - Attribute Directive dynamically modifies the class of an element.
* ```<angularSelector *ngFor="let arrayObject of angularClassInstancePropertyArray>``` - 

[`^ Back to Top`](#contents)

## Templates
 - **Template References** - ```<element #referenceName>``` Now you can refer to this value and pass it ONLY within the same template.


[`^ Back to Top`](#contents)

## Services

[`^ Back to Top`](#contents)

## Dependency Injection

[`^ Back to Top`](#contents)

## Routing

[`^ Back to Top`](#contents)

## Observables

[`^ Back to Top`](#contents)

## Forms

[`^ Back to Top`](#contents)

## Pipes

[`^ Back to Top`](#contents)
