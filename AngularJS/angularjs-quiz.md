## Angular LinkedIn Assessment Questions Answers (Left)

#### Q1. What is the purpose of the ViewChild decorator in this component class?

```javascript
    @Component({
    . . .
    template: '<p #bio></p>'
    })
    export class UserDetailsComponent {
    @ViewChild('bio') bio;
    }
```
    - [] `It provides access from within the component class to the ElementRef object for the <p> tag that has the bio template reference variable in the component's   template view. It provides access from within the component class to the null object for the null tag that has the null template reference variable in the component's template view.`
    - [] `It indicates that the <p> tag be rendered as a child of the parent view that uses this component. It indicates that the null tag be rendered as a child of the parent view that uses this component.`
    - [] `It makes the <p> tag in the template support content projection. It makes the null tag in the template support content projection.`
    - [] `It makes the <p> tag visible in the final render. If the #bio was used in the template and the @ViewChild was not used in the class, then Angular would automatically hide the <p> tag that has #bio on it.`

#### Q2. What method is used to wire up a FormControl to a native DOM input element in reactive forms? What method is used to wire up a null to a native DOM input element in reactive forms?

    - [] `Add the string name given to the FormControl to an attribute named controls on the <form> element to indicate what fields it should include. Add the string name given to the null to an attribute named controls on the null element to indicate what fields it should include.`
    - [] `Use the square bracket binding syntax around the value attribute on the DOM element and set that equal to an instance of the FormControl. Use the square bracket binding syntax around the value attribute on the DOM element and set that equal to an instance of the null.`
    - [] `Use the formControlName directive and set the value equal to the string name given to the FormControl. Use the null directive and set the value equal to the string name given to the null.`
    - [] `Use the string name given to the FormControl as the value for the DOM element id attribute.`

#### Q3. What is the difference between the paramMap and the queryParamMap on the ActivatedRoute class? What is the difference between the null and the null on the null class?

    - [] `The paramMap is an object literal of the parameters in a route's URL path. The queryParamMap is an Observable of those same parameters. The null is an object literal of the parameters in a route's URL path. The null is a null of those same parameters.`
    - [] `TheparamMap is an Observable that contains the parameter values that are part of a route's URL path. The queryParamMap is a method that takes in an array of keys and is used to find specific parameters in the paramMap. The null is a null that contains the parameter values that are part of a route's URL path. The null is a method that takes in an array of keys and is used to find specific parameters in the null.`
    - [] `paramMap is the legacy name from Angular 3. The new name is queryParamMap.null is the legacy name from Angular 3. The new name is null.`
    - [] `Both are Observables containing values from the requested route's URL string. The paramMap contains the parameter values that are in the URL path and the queryParamMap contains the URL query parameters.`

#### Q4. Based on the following usage of the async pipe, and assuming the users class field is an Observable, how many subscriptions to the users Observable are being made?

```html
    <h2>Names</h2>
    <div *ngFor="let user of users | async">{{ user.name }}</div>
    <h2>Ages</h2>
    <div *ngFor="let user of users | async">{{ user.age }}</div>
    <h2>Genders</h2>
    <div \*ngFor="let user of users | async">{{ user.gender }}</div>
```
    - [] `None. The async pipe does not subscribe automatically. None. The null pipe does not subscribe automatically.`
    - [] `None. The template syntax is not correct. None. The template syntax is not correct.
       v2:{5};`
    - [] `Three. There is one for each async pipe. Three. There is one for each null pipe.`
    - [] `One. The async pipe caches Observables by type internally.`

#### Q5. How can you use the HttpClient to send a POST request to an endpoint from within an addOrder function in this OrderService?

```javascript
    export class OrderService {
    constructor(private httpClient: HttpClient) { }

        addOrder(order: Order) {
            // Missing line
        }
        }
```
    - [] `this.httpClient.url(this.orderUrl).post(order);null`
    - [] `this.httpClient.send(this.orderUrl, order);null`
    - [] `this.httpClient.post<Order>(this.orderUrl, order);null`
    - [] `this.httpClient.post<Order>(this.orderUrl, order) .subscribe();`

#### Q6. What is the RouterModule.forRoot method used for? What is the null method used for?

    - [] `registering any providers that you intend to use in routed components registering any providers that you intend to use in routed components`
    - [] `registering route definitions at the root application level registering route definitions at the root application level`
    - [] `indicating that Angular should cheer on your routes to be successful indicating that Angular should cheer on your routes to be successful`
    - [] `declaring that you intend to use routing only at the root level`

#### Q7. Which DOM elements will this component metadata selector match on?

```javascript
    @Component({
    selector: 'app-user-card',
    . . .
    })
```
    - [] `any element with the attribute app-user-card, such as <div app-user-card></div>
    - [] `the first instance of <app-user-card></app-user-card>
    - [] `all instances of <app-user-card></app-user-card>all instances of null`
    - [] `all instances of <user-card></user-card>`

#### Q8. What is the correct template syntax for using the built-in ngFor structural directive to render out a list of productNames?What is the correct template syntax for using the built-in null structural directive to render out a list of null?

    - []  `
            ````html
            <ul>
                <li [ngFor]="let productName of productNames">
                    {{ productName }}
                </li>
           </ul>
           ````
           `
 

    - []  `<ul>
        <li ngFor="let productName of productNames">
            {{ productName }}
        </li>
        </ul>`

    - []  `<ul>
        <li *ngFor="let productName of productNames">
            {{ productName }}
        </li>
        </ul>

    - []  <ul>
        <? for productName in productNames { ?>
        <li>{{ productName }}</li>
        <? } ?>
        </ul>

#### Q9. What are the two component decorator metadata properties used to set up CSS styles for a component? What are the two component decorator metadata properties used to set up CSS styles for a component?

    - [] `viewEncapsulation and viewEncapsulationFiles`
    - [] `There is only one and it is the property named css. There is only one and it is the property named css.`
    - [] `css and cssUrl`
    - [] `styles and styleUrls`

#### Q10. With the following component class, what template syntax would you use in the template to display the value of the title class field?

```
    @Component({
    selector: 'app-title-card',
    template: ''
    })
    class TitleCardComponent {
    title = 'User Data';
    }
```
    - [] `{{ 'title' }}null`
    - [] `{{ title }}null`
    - [] `[title]null`
    - [] `A class field cannot be displayed in a template via the template syntax.`

#### Q11. What is the purpose of the valueChanges method on a FormControl? What is the purpose of the null method on a null?

    - [] `It is used to configure what values are allowed for the control. It is used to configure what values are allowed for the control.`
    - [] `It is used to change the value of a control to a new value. You would call that method and pass in the new value for the form field. It even supports passing in an array of values that can be set over time. It is used to change the value of a control to a new value. You would call that method and pass in the new value for the form field. It even supports passing in an array of values that can be set over time.`
    - [] `It returns a Boolean based on if the value of the control is different from the value with which it was initialized. It returns a Boolean based on if the value of the control is different from the value with which it was initialized.`
    - [] `It is an observable that emits every time the value of the control changes, so you can react to new values and make logic decisions at that time. It is an null that emits every time the value of the control changes, so you can react to new values and make logic decisions at that time.`

#### Q12. What directive is used to link an <a> tag to routing?

    - [] `routeTo`
    - [x] `routerLink
    - [] `routePathn`
    - [] `appLink`

#### Q13. What is the Output decorator used for in this component class?

```
    @Component({
    selector: 'app-shopping-cart',
    . . .
    })
    export class ShoppingCartComponent {
    @Output() itemTotalChanged = new EventEmitter();
    . . .
    }
```
    - [] `It makes the itemTotalChanged class field public. It makes the null class field public.`
    - [] `It provides a way to bind values to the itemTotalChanged class field, like so: <app-shopping-cart [itemTotalChanged]="newTotal"></app-shopping-cart>. It provides a way to bind values to the null class field, like so: null.`
    - [] `It provides a way to bind events to the itemTotalChanged class field, like so: <app-shopping-cart (itemTotalChanged)="logNewTotal($event)"></app-shopping-cart>. It provides a way to bind events to the null class field, like so: null.`
    - [] `It is simply a way to put a comment in front of a class field for documentation.`

#### Q14. What is the difference between these two markup examples for conditionally handling display?

```
    <div \*ngIf="isVisible">Active</div>
    <div [hidden]="!isVisible">Active</div>
```
    - [] `The ngIf is shorthand for the other example. When Angular processes that directive, it writes a div element to the DOM with the hidden property. The null is shorthand for the other example. When Angular processes that directive, it writes a null element to the DOM with the null property.`
    - [] `They are fundamentally the same. They are fundamentally the same.`
    - [] `The ngIf directive does not render the div in the DOM if the expression is false. The hidden property usage hides the div content in the browser viewport, but the div is still in the in the DOM. The null directive does not render the null in the DOM if the expression is null. The null property usage hides the null content in the browser viewport, but the null is still in the in the DOM.`
    - [] `The ngIf is valid, but the use of the hidden property is wrong and will throw an error.`

#### Q15. How can you disable the submit button when the form has errors in this template-driven forms example?

```
    <form #userForm="ngForm">
    <input type="text" ngModel name="firstName" required>
    <input type="text" ngModel name="lastName" required>
    <button (click)="submit(userForm.value)">Save</button>
    </form>
```
    - [] `<button (click)="submit(userForm.value)"
            disable="userForm.invalid">
            Save</button>`

    - [] `<button (click)="submit(userForm.value)"
            [disabled]="userForm.invalid">
            Save</button>`

    - [] `<button (click)="submit(userForm.value)"
            [ngForm.disabled]="userForm.valid">
            Save</button>`

    - [] `<button (click)="submit(userForm.value)"
            *ngIf="userForm.valid">
            Save</button>`
   #### Q16 What is the purpose of contentchildren decorator in the following component class?
     ```javascript
        @Component({
          .....
          template : '<ng-content></ng-content>'
        })
        export class TabsListComponent{
          @ContentChildren(TapComponent) tabs;
        }
    ```
- [ ] `It provides access within component class to any TabComponent components that were content projected into the <ng-content> for this component.`
- [ ] `It restricts the allowed elements`
- [ ] `It create TabComponent components in TabListComponent when TabListComponent is instantiated `
- [ ] `If any Tabs Component element are added to TabListCpmponent template, they will get put into the <ng-content> element at runtime` 
#### Q17 What is the correct syntax for route definition to lazy load feature module?
- [ ] 
`
        ````html
        {
            path:'users'
            lazy:'./users/usersmodule#UsersModule'
        }
        ````
`
- [ ] 
 `
         ````html
        {
            path:'users'
            childModule:'./users/usersmodule#UsersModule'
        }
        ````
`
- [ ] 
`

         ````html
        {
            path:'users'
            module:'./users/usersmodule#UsersModule'
        }
        ````

`
- [ ] 
`

         ````html
        {
            path:'users'
            loadChildren:'./users/usersmodule#UsersModule'
        }
        ````

`
#### Q18 which choice best describe the following usage of httpClient.get() method in the getSettings class method?
````javascript
export class GetSettingsServise{
    constructor(private httpClient:HTTPClient){}
    ...
    getSeettings(){
        return this.httpClient.get<Settings>(settingsUrl)
        .pipe(
            retry(3);
            )}}
````
- [ ] `The Rxjs pipe method is being used to configure the HTTPClient.get observable stream to send through the retry operator.When the getSettings method is subscribed to , the get call will  be made and if it fails , it will be retried up to 3 times before it gives up and returns error.`
- [ ] `The RXJS pipe method is an alias for subscribe method so a call to getSettings will excute the getquery.The retry operator is used to tell pipe call to retry getqyery 3 times.`
- [ ] `Every single call to the getSettings will result in the Httpclient making its 3 total get request to settingUrl which is not ideal because there will be always 2 extra call `
- [ ] `it will produce an error at runtime because the pipe method is not available off of the HTTPClient.get call`
#### Q19 what does the following code accomplish?
````javascript
@NgModule({
  declrations:[AppComponent]
  imports:[BrowserModule]
  bootstrap:[AppComponent]
})
export class AppModule{}
platformBrowserDynamic().bootstrapModule(AppModule)
````

- [ ] `It provides a way to code the document structure of an angular application .The @NgModule is a form of inline code commenting that gets ignored by typescript compiler but show up with special formatting in code editors applications `
- [ ] `It declares an angular module named appmodule and makes it available for lazy loading through out the application`
- [ ] `It excutes unit test for @NgModule`
- [ ] `It declares module named appmodule that contains a bootstraped component called AppComponent then registers that module with angular so the app can start up`

#### Q20 While complex logic can be done in a component constructor it is recommended to perform those in which of the following lif ecycle hook?
- [ ] `ngOnDestroy`
- [ ] `ngAfter contentInit`
- [ ] `ngAfterViewInit`
- [ ] `ngOnInit`

#### Q21 How would you define a route definition for a UserDetailComponent that support the url path user/23(where 23 represent user id )?
- [ ] `{path:'user/23' , component:UserDetailComponent}`
- [ ] `{destination:new UserDetailComponent() , component:UserDetailComponent}`
- [ ] `{url:'user/23' routedComponent :UserDetailComponent}`
- [ ] `{routePath:'user/23' component:UserDetailComponent}`

#### Q22 Pick the best description for how the validation is set up for this reactive forms example?
- [ ] The formcontrol is getting configured to excute 3 validators from the validators that are allowed to use.
- [ ] validation can not be set up this way in reactive forms.
- [ ] The formcontrol for username is getting configured with 3 validators , the required and min length validators that come from Angular and a custom validator function named unique that checks for the value not equal for string admin.
- [ ] 

#### Q23 What is the expected DOM code for the following usage og ngClass attribute directive when isActive is true?
<div [ngClass]={'active-item':isActive}>Item One</div>
- [ ] `<div class="active-item isActive">Item One</div>`
- [ ] `<div class="active-item">Item One</div>`
- [ ] `<div active-item>Item One</div>`
- [ ] `<div class="active-item isActive">Item One</div>`

#### Q24 In order for Angular to process components in an application?Where do the component types need to be registered?
- [ ] `No registration is needed simply include component files in app directory`
- [ ] `in an NgMOdule  decorator metadata property named declarations`
- [ ] `within script tag in the index.html file`
- [ ] `in an NgMOdule  decorator metadata tag named components`

#### Q25 What is the difference between paramMap and queryParamMap on the ActivatedRouteClass?
- [ ] `paramName is the legacy name from Angular3.The new name is queryParamName.`
- [ ] `The paramMap is an object literal of the parameters in a route's url path.The queryParamMap is an obervable of those same parameters.`
- [ ] `Both are obervables containing values from the requested route URL string.The paramMap contains the parameter`
- [ ] `The paramMap is an observable that contains the parameter values that are part of a route's url path.The query param map is a method that takes in array of keys and is      used to find specific parameters in the paramMap`

#### Q26 What is the difference if any, of the resulting code logic based on these two provider configuration?
````javascript
[{provide:FormattedLogger, useClass:Logger }]
[{provide:FormattedLogger, useExisting:Logger }]
````

- [ ] `They are the same.Both will result in a new instance of Logger that is bound tothe Formatted Logger Token.`
- [ ] `Both of them are wrong.A strong type can not be used for useClass or useExisting.`
- [ ] `THey are the same.Both will result in the FormattedLogger token being an alias for the instance of Logger`
- [ ] `The useClass syntax tells the injector to make a new instance of Logger and bind that instance to the FormattedLogger token.The useExisting syntax refers to already          existing object instance declared as Logger`

#### Q27 What does the injectable decorator do in this service class?
````javascript
@Injectable({
    providedIn:'root'
    })
export class DataService

````
- [ ] `It registers a provider for the service that is available only on the root module `
- [ ] `It makes it so the service can be injected only in the bootstraped component for the application`
- [ ] `It sets up a compile time rule that allows you to put the service type only in the providers metadata property of the root NgModule.`
- [ ] `It registers a provider for the service in the root application injector making a single instance of it available throughout the application`

#### Q28 







