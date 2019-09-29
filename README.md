# Anatomy of an Angular application:
components + services  
component = 
- template (html, bindings & directives): VIEW
- class (code for the view, Typescript, properties for the view, methods): MODEL
- metadata (additional information about the component, defined with a decorator)

Modules group components together. An angular app has at least the root module. Modules generally corespond to application features.

# Typescript
- transpiles to JavaScript
- Typescript type definition files: *.d.ts
- uses class-based OOP

# Setting up the environment
- install npm (it's bundled with node.js)
- set up an Angular application (this course starts with a github repo: app is created with angular cli)
  - manually
  - Angular CLI 

## App structure
- src/app: source code
- package.json: app dependencies (use "npm install" to install these libraries); if cert error use "npm config set registry http://registry.npmjs.org/" first, then "install"; 
- to install bootstrap & font awesome: "npm install bootstrap font-awesome";
- npm start: start the app (run from APM dir - where package.json is located): executes the script in package.json file "ng serve -o".
- ctrl + c stops the server

# Modules
Angular uses ES2015 modules. Angular modules are different than ES modules. They help organize the app.

# Components  
Componenet example: app.component.ts (includes both view & model).  
Component name convention: "NameComponent". The root component is called, by convention "AppComponent".
Decorator: function that adds metadata to a class, its methods or method arguments. (@DecoratorName). Receives an object as argument:
- selector: defines the directive (custom html tag) name used to reference the component in html.
- template: html to render & data bindings {{propertyName}}

Bootstrapping components: 
- add them as directives to the index.html
- add them to modules (see app.module.ts): @NgModule defines this as a module, bootstrap property defines startup component

# Templates, Interpolation and Directives  

Templates can be defined:
- inline: template: "html here" or on multiple rows using backticks ``
- linked: templateUrl: 'path to html file'

Data bindings:
- interpolation (one way: property -> template): {{propertyName}}
- two way:

Event binding:

Angular built-in Directives:
- structural: *ngIf, *ngFor (defined in BrowserModule)



**Progress:** Data bindings & pipes: Property binding


# Stuff to add to resume:
- Modules, Components, Directives, Templates, Data binding
- Services
- Typescript
- Bootstrap 4
- 
