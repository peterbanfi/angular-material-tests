# Steps

### Set up
> 1. ng new nameOfProject --routing --style=scss
> 2. yarn add @angular/material @angular/cdk @angular/animations hammerjs --dev
> 3. yarn add @angular/animations --dev
> 4. yarn add hammerjs --dev

### Set up 2
> 1. main.ts --> import 'hammerjs'; 
> 2. app.module.ts -->
```typescript
 import {BrowserAnimationsModule} from '@angular/platform-browser/animations';
```

### Create materials file
> 1. material.ts
> 2. boiler plate: 
```typescript
 import {MatButtonModule, MatCheckboxModule} from '@angular/material';
 import {NgModule} from '@angular/core';

 @NgModule({
     imports: [MatButtonModule, MatCheckboxModule],
     exports: [MatButtonModule, MatCheckboxModule],
 })
 export class MyOwnCustomMaterialModule {}
```
> 3. import material.ts to app.module.ts!
> 4. Ha egy material design elemet akarok hozzáadni, akkor mindig behelyezem a material.ts-be!

### Create theme
> 1. styles.scss
```typescript
 @import '~@angular/material/prebuilt-themes/indigo-pink.css';
```
> Or custom themes: https://material.angular.io/guide/theming

### Add icons

> 1. https://google.github.io/material-design-icons/
> ```html
<link href="https://fonts.googleapis.com/icon?family=Material+Icons"
      rel="stylesheet">
```

### Add components!

> 1. https://material.angular.io/components/categories

# NgRx

> This is based on https://itnext.io/ngrx-best-practices-for-enterprise-angular-applications-6f00bcdf36d7