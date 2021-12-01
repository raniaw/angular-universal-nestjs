# angular-universal-nestjs

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version ~13.0.0.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).

## created a clean angular project.

## install @nguniversal/express-engine
npm i --save @nguniversal/express-engine

## modified node_modules/@nguniversal/express-engine/package.json

removed "type": "module" and

added in exports the following:
    "./schematics/utils": {
      "types": "./schematics/utils/index.d.ts",
      "esm2020": "./schematics/utils/index.js",
      "es2020": "./schematics/utils/index.js",
      "es2015": "./schematics/utils/index.js",
      "node": "./schematics/utils/index.js",
      "default": "./schematics/utils/index.js"
    }
After this I run ng add @nestjs/ng-universal. Things are different this time and everything installs correctly and the server files are correctly installed.

## start dev:ssr

npm run dev:ssr 

##  build

npm run build:ssr

## start server

npm run serve:ssr

## localhost

http://localhost:4000
