# RoutingApp

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 10.0.3.


## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

#### 0. Generate app with routing
`ng new app-name --routing`
<br>
Core files to work with are:
- AppRoutingModule
- AppModule

#### 1. Import all components into AppRoutingModule

- N.B if you generated first component as follows 
`ng g c first`
it will be registered with a class FirstComponent in PascalCase inside first.component.ts file in first folder. 
will be referenced as ff:
`import { FirstComponent } from './first/first.component';`


#### 2. Import the AppRoutingModule into AppModule and add it to the imports array
- N.B The CLI peforms this for you since the --routing flag was used 

#### 3. Define routes in Routes array in AppRoutingModule
`[{path: 'first-component', component: FirstComponent}, {}...]`

#### 4. Add routes links in the app html
   `<li><a routerLink="/first-component" routerLinkActive="active">First Component</a></li>`
    `<li><a routerLink="/second-component" routerLinkActive="active">Second Component</a></li>` 