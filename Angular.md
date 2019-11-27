


<h1 align="center">ANGULAR</h1>
<p align="center">
    <img width="200px" src=https://raw.githubusercontent.com/AndresMWeber/WebDefinitions/master/media/Angular.png>
</p>

# Contents
[`Components`](#components)

[`ngModules`](#ngModules)

[`Databinding`](#databinding)

[`Directives`](#directives)

[`Services`](#services)

[`Dependency Injection`](#dependency-injection)

[`Routing`](#routing)

[`Observables`](#observables)

[`Forms`](#forms)

[`Pipes`](#pipes)

## Components
Angular uses a **decorator** in order to wrap whatever class you create as a component.  This contrasts with **React's** ```extend``` style class definition.  You pass an ```object``` that has an optional ```selector``` and a ```templateUrl``` or ```template``` field that specifies the html file that contains its skeleton.  

Angular also has a CLI tool that allows you to generate the scaffolding for any given component using ```ng generate component``` among many other features.

[`^ Back to Top`](#contents)

## ngModules

* You can scaffold a component using ```ng generate component *componentName*```
* Must specify a template/templateUrl


[`^ Back to Top`](#contents)

## Databinding
* **String Manipulation** - ```{{propertyName}}```

* **Property Binding** - ```[htmlProperty ]="angularClassProperty"``` - Derives the value of the angular class instance property that you set the html element's property equal to.

* **Event Binding** - ```(eventName)="angularClassMethod()"``` - Allows to bind a DOM element's event to the Angular class instance method.

* **Two-Way Databinding** - ```([ngModel])="angularClassPropertyToBind``` - Allows two way bound class properties that can be set from the html element or from the angular class instance property.

[`^ Back to Top`](#contents)

## Directives
Directives are a class like a component but without a view or template that modify their host elements based on new abilities provided by the directives.
* ```*ngIf="conditionalExpression" (#elseCondition)``` - Structural Directive that allows conditional DOM manipulation.
* ```*ngFor=let element of iterable; let i = index``` - Structural Directive that allows iterable DOM manipulation.
* ```[ngStyle]=``` - Attribute Directive dynamically modifies the appearance/styling of an element.
* ```[ngClass]={className: boolean expression}``` - Attribute Directive dynamically modifies the class of an element.
* ```<angularSelector *ngFor="let arrayObject of angularClassInstancePropertyArray>``` - 

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
