angular-bootbox
===============

makeusabrew/bootbox (https://github.com/makeusabrew/bootbox) to AngularJS

### Scripts

```html
<script type="text/javascript" src="http://cdnjs.cloudflare.com/ajax/libs/bootbox.js/4.2.0/bootbox.js"></script>
<script src="scripts/angular-bootbox.js"></script>
```

### App

```js
var app = angular.module('YourApp', ['angular-bootbox']);
```

```js
app.config(function ($bootboxProvider) {
  $bootboxProvider.setDefaults({ locale: "es" });
});
```

### Controller

```js
app.controller('eventsController', ['$scope', 'bootbox', function ($scope, bootbox) {
bootbox.confirm("Are you sure?", function (result) {
    return true;
});
```
