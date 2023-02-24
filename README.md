# angular-15-jsdom

This is a demo of Angular 15.2.0 with unit tests running under jsdom.

Look at contents of patches/ folder to see which patches we have had to apply to make it work.

Instructions:
1. Run `npm install`
2. Run `npm run test:chrome` and all three tests should pass.
3. Run `npm run test:jsdom` and it should time-out.
4. Run `npm run patch-package`
5. Run `npm run test:jsdom` again and now it works.

Your output in step 5 should look like this:  
* AppComponent
    √ should render title
    √ should create the app
    √ should have as title 'angular-15-json'
There will also be an error message in red: "Error: TypeError [ERR_INVALID_PROTOCOL]" - you can safely ignore this.

----------

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 15.2.0.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The application will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via a platform of your choice. To use this command, you need to first add a package that implements end-to-end testing capabilities.

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.io/cli) page.
