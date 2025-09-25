# Getting Started with Create Angular App

This project was created using:
### `ng new <project-name>`
Enable routing by typing : y
Stylesheet Choice: CSS 

## Available Scripts

In the project directory, you can run:

### `ng serve -o`

Runs the app in the development mode.\
-o flag opens the browser automatically or Else use
Open [http://localhost:4200](http://localhost:4200) to view it in the browser.

## Project Structure

CRUD: Create, Read, Update, and Delete
App Root -> Router -> {Module1[...Components], Module2[...Components]} -> Service

### `ng generate module <module-name>`

Generates module 

### `ng generate component <component-name> --module=<module-name>`

Generates component and declared inside module, component can only be declared by a single component

### `ng generate service <service-name>`

Generates service, kind of stand-alone and not part of module

### `ng generate interface models/<interface-name>`

Generates model

### Router
App-routing.module.ts: Add route to routes array as 
path, component

Edit Route: {path: "edit/:id", component: <component-name>}
html: [routerLink]="['edit', id]"
module: import RouterModule

Read Route Value:
component: import ActivatedRoute, 
id = activatedRoute.snapshot.paramMap.get('id'); // and patchValue

