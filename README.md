# From YouTube video: Getting Started with Angular 6 Material (Tutorial)
[![Getting Started with Angular 6 Material (Tutorial)](https://i.ytimg.com/vi/Fcr-gM-QThc/hqdefault.jpg)](http://www.youtube.com/watch?v=Fcr-gM-QThc)

## Create project and setup to use Angular Material

```$ ng new material-ng --routing --style=scss```

```$ npm i @angular/material @angular/cdk```

```$ npm i @angular/animations```

```$ npm i hammerjs```

### *main.ts*
```js
import "hammerjs";
```

### *app.module.ts*
```js
import { BrowserAnimationsModule } from '@angular/platform-browser/animations';
```

... and add to imports

### create *material.ts* in the *app* folder
```js
import { MatButtonModule, MatCheckboxModule } from '@angular/material';
import { NgModule } from '@angular/core';

@NgModule({
  imports: [MatButtonModule, MatCheckboxModule],
  exports: [MatButtonModule, MatCheckboxModule],
})
export class MaterialModule {}
```

### *app.module.ts*
```js
import { MaterialModule } from './material';
```
... and add to imports

### *styles.scss*
```js
@import "~@angular/material/prebuilt-themes/indigo-pink.css";
```
### *index.html*
```js
<link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet">
```

---

