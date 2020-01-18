


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
Angular uses a **
** in order to wrap whatever class you create as a component.  This contrasts with **React's** ```extend``` style class definition.  You pass an ```object``` that has an optional ```selector``` and a ```templateUrl``` or ```template``` field that specifies the html file that contains its skeleton.  

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

* **Property Binding** - ```[htmlProperty ]="angularClassProperty"``` - Directly binds the value of the angular class instance property to the specified html element's property as depicted in between the brackets.

* **Event Binding** - ```(eventName)="angularClassMethod()"``` - Allows to bind a DOM element's event to the Angular class instance method.  Can optionally pass ```$event``` as a parameter to gain access to the event data.

* **Two-Way Databinding** - ```([ngModel])="angularClassPropertyToBind``` - Allows two way bound class properties that can be set from the html element or from the angular class instance property. ()+[] combines both both property and event binding.  But you need to add the FormsModule to add the two way databinding directives.

* **Custom Property Binding (Input)** - (in Angular view component class definition) ```@Input('customPropertyAlias') property``` - Now you can bind to this property anywhere in the angular html view files.  To add an alias to these properties, just pass a string in the Input decorator as a string (not recommended unless necessary).

* **Custom Property Binding (Output)** - (in Angular view component class definition) ```@Output() property = new EventEmitter``` - This enables triggering the property as an event emitter and passing data to the parent component as output.

``` javascript
import { Component, Input, EventEmitter, Output } from '@angular/core';
@Component({
    template: '<article class="product" (click)="onClicked()"><div {{ productName }}</div></article>',
    selector: 'app-product',
})
export class ProductComponent {
    @Output() productClicked = new EventEmitter();
    @Input() productName: string;
    onClicked () {
        this.productClicked.emit()
    }
```
``` html
<!-- Enclosing component's html template using the previously defined Angular Component above -->
<app-product 
             *ngFor="let product of products" 
             (productClicked)="onRemoveProduct(product)" <!-- This will allow the parent component to listen to the event and trigger a response-->
             [productName]="product"
</app-product>
```


[`^ Back to Top`](#contents)

## Directives

Directives are a class like a component but without a view or template that modify their host elements based on new abilities provided by the directives.
Two Types of Directives:
1. ```Attribute``` - (HTMLElement) Only affects/changes the element they are added to
2. ```Structural``` - (*HTMLElement) Affects the whole area in the DOM (elements are added/removed). (Can only have one per element)

* ```*ngIf="conditionalExpression" (#elseCondition)``` - Structural Directive that allows conditional DOM manipulation.
* ```*ngFor=let element of iterable; let i = index``` - Structural Directive that allows iterable DOM manipulation.  Within the rest of that html tag you can refer to the ```element``` name as a variable.
* ```[ngSwitch]="value"'``` ```<subElement *ngSwitchCase="5">``` - Based on "value" property of the Angular Component you can conditionally show specific sub HTML elements.
* ```[ngStyle]=``` - Attribute Directive dynamically modifies the appearance/styling of an element.
* ```[ngClass]={className: boolean expression}``` - Attribute Directive dynamically modifies the class of an element.
* ```<angularSelector *ngFor="let arrayObject of angularClassInstancePropertyArray>``` - 

Custom Directive that colors background color green :
```javascript
import { Directive, ElementRef, OnInit } from '@angular/core';

@Directive({
    selector: '[customSelectorName]`
})
export class CustomDirectiveClass {
    constructor(private elementRef: ElementRef){
    }
    
    ngOnInit() {
        this.elementRef.nativeElement.style.backgroundColor = 'green';
    }
}
// NOTE: Must add Custom Directive class to App module declarations.
```

Custom Directive that colors background color green using Renderer2:
```javascript
import { Directive, ElementRef, OnInit, Renderer2 } from '@angular/core';

@Directive({
    selector: '[customSelectorName]`
})
export class CustomDirectiveClass {
    constructor(private elementRef: ElementRef, private renderer: Renderer2){
    }
    
    ngOnInit() {
        this.renderer.setStyle(this.elementRef.nativeElement, 'background-color', 'green');
    }
}
// NOTE: Must add Custom Directive class to App module declarations.
```

Custom Directive that colors background color blue on mouse over permanently using HostListener
Also binds a backgroundColor property from elementRef.nativeElement.style.backgroundColor. 
If you want to have input must supply Input with the same selector name and now refer to the Custom Directive as ```[customDirective]="overrideValue"```

```javascript
import { Directive, ElementRef, OnInit, Input, HostBinding } from '@angular/core';

@Directive({
    selector: '[customSelectorName]`
})
export class CustomDirectiveClass {
    () defaultColor: string = 'transparent';
    @Input('customSelectorName') highlightColor: string = 'blue';
    @HostBinding('style.backgroundColor') backgroundColor: string = this.highlightColor;
    
    constructor(private elementRef: ElementRef, private renderer: RendererV2){
    }
    
    ngOnInit() {
        this.backgroundColor = this.defaultColor
    }
    
    @HostListener('mouseenter') mouseover(eventData: Event){
        this.backgroundColor = this.highlightColor;
    }
}
// NOTE: Must add Custom Directive class to App module declarations.
```
[`^ Back to Top`](#contents)

## Forms
1.  Should not have an action, but instead uses the (ngSubmit) event handler provided by Angular.  
2.  You do not need two way binding and instead can just add ngModel to any input fields to automatically add two way binding after defining the name on the html tag.  
3.  You have to add the javascript form object by adding a local reference with the # syntax which will give us access to the implicitly created form object that was created behind the scenes.

```html
<!-- products.component.html -->
<h1>My Products</h1>
<form (ngSubmit)="onAddProduct()" #f="ngForm"> <!-- Gives us access to the forms object angular created -->
    <input type="text" ngModel name="productName" required>
    <button type="submit">Add Product</button>
</form>
<app-product (productClicked)="onRemoveProduct(product)" 
```
```javascript
// products.component.ts
import { Component, Input, EventEmitter, Output } from '@angular/core';
@Component({
    template: '<article class="product" (click)="onClicked()"><div {{ productName }}</div></article>',
    selector: 'app-products',
})
export class ProductComponent {
    @Output() productClicked = new EventEmitter();
    @Input() productName: string;
    onAddProduct(form){
        console.log(form) // this will print out the DOM form object.
        if (form.valid) {
            this.products.push(form.value.productName) // productName is available as a control because we added ngModel + name="productName" in the html file.
        }
    }
    onRemoveProduct(productName: string) {
        this.products = this.products.filter(p => p !== productName)
    }
```
[`^ Back to Top`](#contents)

## Templates
 - **Template References** - ```<element #referenceName>``` Now you can refer to this value and pass it ONLY within the same template.


[`^ Back to Top`](#contents)

## Services
A service class is a class meant to be instantiated and passed as an argument to be an interface for retrieving external data for a component.  After defining a service class you need to add it to the app.module.ts providers array in order to have it injectable to your App's components.  That way just by defining it as an type casted parameter in the constructor it will automatically provide an automagically bound instance property variable of that class to the component.

Use the ```.next()``` method in order to signal the subscribed objects of changes.

```TypeScript
import { Subject } from 'rxjs';

export class ProductsService {
    private products = ['A Book'];
    productsUpdated = new Subject(); 
    
    addProduct(productName: string) {
        this.products.push(productName);
        this.productsUpdated.next();
    }
    
    getProducts() {
        return [...this.products];
    }
}
```

#### Service Subscriptions
By definiting a Subject instance you add an event emitter that can subscribed to for subsequent changes.
In the encapsulating class that uses the Service as a bound property instance just call
(It is also good practice to store that subscription in an instance variable for cleanup purposes and preventing memory leaks.)

```TypeScript
import { Subscription } from 'rxjs';

// within the class body:
    private productsSubscription: Subscription
    
    // within subscription function (probably ngOnInit)
        this.productsSubscription = this.productsService.productsUpdated.subscribe(() => {
            this.products = this.productsService.getProducts();
        });
    
    // within ngOnDestroy:
        this.productsSubscription.unsubscribe()
```

[`^ Back to Top`](#contents)

## Dependency Injection

[`^ Back to Top`](#contents)

## Routing
```TypeScript
// home.component.ts
import { Component } from '@angular/core'

@Component({
    template: '<h1>The Home Component</h1>'
})
export class HomeComponent {}
```

```TypeScript
// app-routing.module.ts
import { NgModule } from '@angular/core'
import { Routes, RouterModule } from '@angular/router'
import { HomeComponent } from './home.component'
import { ProductsComponent } from './products.component'

const routes: Routes = [
    { path: '', component: HomeComponent},
    { path: 'products', component: ProductsComponent},
];

@NgModule({
    imports: [
        RouterModule.forRoot(routes)
    ],
    exports: [RouterModule]
})
export class AppRoutingModule {}
```

Then import the AppRoutingModule in app.module.ts in the imports section of the NgModule decorator.
Now you can feel free to use the router using html and the ```routerLink directive```:
```html
<h1>My App</h1>
<a routerLink="/">Home</a>
<a routerLink="/products">Products</a>
<router-outlet></router-outlet>
```
[`^ Back to Top`](#contents)

## Observables

[`^ Back to Top`](#contents)

## Pipes

[`^ Back to Top`](#contents)
