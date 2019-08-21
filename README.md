# Anatomy of an Angular application:
components + services  
component = 
- template (html view, bindings & directives) 
- class (code for the view, Typescript, properties for the view, methods) 
- metadata (additional information about the component)

Modules group components together. An angular app has at least the root module. Modules generally corespond to application features.

# Typescript
- transpiles to JavaScript
- Typescript type definition files: *.d.ts
- uses class-based OOP

# Setting up the environment
- install npm (it is bundled with node.js)
- set up Angular application
  - manually
  - Angular CLI

## App structure
- src/app: source code
- package.json: app dependencies (use "npm install" to install these libraries); if cert error use "npm config set registry http://registry.npmjs.org/" first, then "install"; npm start: start the app

# Modules
Angular uses ES2015 modules. Angular modules are different than ES modules. They help organize the app.

# Components

Progress: Bootstrapping our app component
