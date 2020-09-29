# MyContractUi

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 10.1.3.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

Run `npm run-script test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Using Jest
This sample is using Jest instead of Karma and Jasmine combination.

### Add jest jest-preset-angular @types/jest
```console
npm i -D jest jest-preset-angular @types/jest
```

### Add setupJest.ts under src folder and add contents
```console
import 'jest-preset-angular';
```

### Update package.json with jest property

```console
  "jest": {
    "preset": "jest-preset-angular",
    "setupFilesAfterEnv": [
      "<rootDir>/src/setupJest.ts"
    ]
  }
```

### Update package.json script

```console
  "scripts": {
    "ng": "ng",
    "start": "ng serve",
    "build": "ng build",
    "test": "jest",
    "test:watch": "jest --watch",
    "lint": "ng lint",
    "e2e": "ng e2e"
  },
```

### Remove jasmine related packages

```console
npm uninstall jasmine @types/jasmine
```

### Remove karma related packages

```console
npm uninstall karma-jasmine-html-reporter karma-jasmine karma-coverage-istanbul-reporter  karma-chrome-launcher karma
```

### Remove test.ts

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).
