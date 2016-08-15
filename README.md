# ngExam
> An AngularJS 1.x exam from beginner to expert created by [@gdi2290](https://twitter.com/gdi2290)


* What's MVC architecture? 
 * Model - The lowest level of the pattern which is responsible for maintaining data.
   View - This is responsible for displaying all or a portion of the data to the user.
   Controller - Software Code that controls the interactions between the Model and View. 
* What's MVVM architecture?
 * MV same as above. The VM acts as an intermediary between the view and the model, and is responsible for handling the view logic. Typically, the view model interacts with the model by invoking methods in the model classes. The view model then provides data from the model in a form that the view can easily use. 
* What's two way binding?
 * Two-way binding means that any data-related changes affecting the model are immediately propagated to the matching view(s), and that any changes made in the view(s) (say, by the user) are immediately reflected in the underlying model. When app data changes, so does the UI, and conversely. (http://stackoverflow.com/questions/13504906/what-is-two-way-binding)
* What's ng-model?
 * The ngModel directive binds an input,select, textarea (or custom form control) to a property on the scope. (https://docs.angularjs.org/api/ng/directive/ngModel) 
* What is `$http`?
 * A service for making AJAX calls via the HTTP protocol
* What is ng-repeat?
 * Used for repeating a set of elements and iterating over a collection. 
* What are `$index`, `$even`, `$odd`, `$first`, and `$last`?
 * http://www.learn-angular.org/#!/lessons/repeaters  
* How would you filter a list via ng-repeat?
* What's the difference between `angular.module('app' , [])` and `angular.module('app')`
 * first one creates a module injecting the dependency modules. second is used to reference the creation of controllers and directives. 
* What are directives (briefly)? 
 * At a high level, directives are markers on a DOM element (such as an attribute, element name, comment or CSS class) that tell AngularJS's HTML compiler ($compile) to attach a specified behavior to that DOM element (e.g. via event listeners), or even to transform the DOM element and its children. (https://docs.angularjs.org/guide/directive) 
* Why would you use ng-submit instead of ng-click in some cases?
 * The ngSubmit directive binds to the submit event in the browser, which is fired when a form is submitted. The ngClick directive allows you to specify custom behavior when an element is clicked. (http://stackoverflow.com/questions/23553071/differences-between-ng-submit-and-ng-click) 
* What's Dependency Injection?
 * Where you do not create the dependencies required instead have the framework provide it to you. (http://stackoverflow.com/questions/130794/what-is-dependency-injection)
* Do other frameworks use dependency injection (even if only for internal use)? Answer: yes (React,Ember)
* How would you inject services and what are the different ways to do so?
 * Passing a dependency as Function Arguments, Passing a dependency as Array Arguments, Passing a dependency using the $inject service (http://www.infragistics.com/community/blogs/dhananjay_kumar/archive/2016/02/28/different-ways-of-injecting-dependency-in-an-angularjs-application.aspx) 
* What's jqLite?
 * jqLite is a tiny, API-compatible subset of jQuery that allows Angular to manipulate the DOM in a cross-browser compatible way. jqLite implements only the most commonly needed functionality with the goal of having a very small footprint. 
* How do you ensure Angular uses jQuery when including them both?
 * To use jQuery , simply ensure it is loaded before the angular.js file.  
* What are promises and how would you use them?
* What's the difference between factory/provider/service/value/constant?
* When would you use each one?
* What are filters?
* Why would you use ng-src, ng-bind, and ng-cloak?
 * http://www.w3schools.com/angular/ng_ng-bind.asp 
 * http://stackoverflow.com/questions/27554765/use-of-ng-src-vs-src 
 * https://docs.angularjs.org/api/ng/directive/ngCloak 
* What's the difference between ng-if and ng-show?
* What phases are there in angular? Answer: config -> bootstrap -> run
* Why would you use `.config()` and `.run()` phase?
* What is ng-app and how does angular bootstrap?
 * https://docs.angularjs.org/guide/bootstrap 
* When would you use `$q.all()`?
 * https://www.jonathanfielding.com/combining-promises-angular/ 
* Where would you make your network calls controller, template, directive, or service and why? (where would you use $http)
* Say that you are going to alert an error where would you put that alert from a network call? Service, controller, template and why? [Answer](https://gist.github.com/gdi2290/b9d34955f0d3bce2c1b6)
* How would you dynamically filter a list with an ng-repeat? (clicking on different filters)
* What's ng-messages and ng-message?
* What's ng-style and ng-class?
* How would you attach something to the header of every http call?
* What is `$scope.$on()` and how would you use it?
 * http://stackoverflow.com/questions/14502006/working-with-scope-emit-and-on 
* What are `$http` interceptors?
* What is `"$locationChangeStart"`?
 * http://stackoverflow.com/questions/26779704/difference-between-locationchangestart-routechangestart-and-statechangestar 
* What's html5Mode?
* How do you turn off cache for a `$http` call?
* What is the `$templateCache`?
 * http://pracujlabs.io/2015/12/28/using-templatecache-in-angularjs.html 
* How would you implement auth as in locking down certain parts of the app? 
* What's ui-router and why use it over ng-route?
* What are states?
* How do you resolve resources via state/route and how would you do so?
* Given 3 nested states, how would you load the most nested one after the root state resolves while allowing the middle state to load asynchronously?
* What types of directives are there? Angular: element, attribute, class (no one uses class)
* What is `$scope`?
* What is `$rootScope`?
* What is `"$destroy"`?
* What's one time binding?
* When and where would you normally use `.$watch()`?
* What's a stateful filter vs a stateless filter?
* What are `.$dirty`, `.$pristine`, `.$valid`, `.$invalid`, and `.$submitted`?
* What's NgModelController? 
* What's FormController?
* What's ng-model-options and why would you use it?
* What are `$validators` and `$asyncValidators`?
* What's the difference between `scope`, `$scope`, and `$rootScope`?
* What's the difference between controller and link directives?
* How do you require a controller in a directive?
* How do you require more than one controller in a directive?
* What's an isolated scope?
* For an isolate scope what are these symbols `?`,`@`,`=`,`&`,`*` in relation to directives
* What are compile/pre-link/post-link phase for directives?
* What is `$interpolate`?
* What is `$compile`?
* What is `$observe`?
* What's transclusion?
* Why would you need transclusion?
* What's `bindToController:` and `controllerAs:` syntax? 
* What are directives and what are components?
* What's the difference between `.$broadcast()`, and `.$emit()`?
* What are `$timeout()` and `$interval()` and how do you cancel them?
* What's dirty checking?
* Do other frameworks use dirty checking? Answer: yes (React,Polymer)
* What is the `.$digest()` loop?
* What's the difference between `.$digest()` and `.$apply()`?
* What are `$watchGroup` and `$watchCollection`?
* What are `$eval`, `$parse` and `$evalAsync`?
* What is `$applyAsync`?
* What's a decorator in relation to angular's module system?
* How would you filter a large list with ng-repeat to include data from the server and client?
* How would you grab the `$injector`/`$scope` from the chrome console?
* Why is there ng-form?
* How would you dynamically create forms?
* What's CSP and how does it relate to angular?
* How do you structure your files for a large team/project?
* How would you use a module loader/bundler such as browserify, webpack, or systemjs with angular?
* How would you asynchronously load angular?
* How would you inject server rendered data into client angular?
* What's a document fragment?
* What's the ShadowDOM?
* What is needed for your angular web app to work with JavaScript disabled?
* What is needed for your angular web app to be rendered on the server to be sent down to the client?
* Generally speaking how would you paraphrase angular?
* How would you progressively enhance your RESTful app with a pub/sub?
* How would you structure your app if you only had a realtime (pub/sub) API (no REST)?
* What are the different ways to architect your angular app?
* What are the pros and cons of each design?
* What are some anti patterns developers tend to fall into while using angular?
* What are the problems currently facing angular1?
* Explain how Angular 2 is solving all of the problems from 1.x
* Demonstrate a few ways to migrate an Angular 1 app to Angular 2
* What's the difference between MVC, MVVM, MVP(SC), MVP(PV), PM, and how does it compare to Flux/Redux architecture?
* How are dependencies handled when testing Angualar controllers and services?
* How is `$scope` injected when testing Angular controllers?
* What is the purpose of wrapping core Angular providers and services in double underscores? ex: `_$rootScope_`?
* Describe the necessary steps to test the Angular `$http` service
* How would you test an `$http` request to a third party API such as Youtube?
* How would you test the data being returned from the API request?
* What frameworks, languages and tools are available for testing in Angular?
* How is $scope used when testing Angular controlers?
* Explain what `$httpBackend` and `$httpBackend.flush` are used for
* Explain what `angular.mock` is used for

___

enjoy — **AngularClass** 

<br><br>

[![AngularClass](https://cloud.githubusercontent.com/assets/1016365/9863770/cb0620fc-5af7-11e5-89df-d4b0b2cdfc43.png  "Angular Class")](https://angularclass.com)
##[AngularClass](https://angularclass.com)
> Learn AngularJS, Angular 2, and Modern Web Development form the best.
> Looking for corporate Angular training, want to host us, or Angular consulting? scott@angularclass.com
