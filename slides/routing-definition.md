##  Routing Definition

```js
var app = angular.module('myServiceModule', []);

app.config(function ($routeProvider, $locationProvider) {
    $routeProvider.
        when('/', {
            templateUrl: 'partials/main',
            controller: 'MainCtrl'
        }).
        when('/hello', {
            templateUrl: 'partials/hello',
            controller: 'HelloCtrl'
        }).
        otherwise({
            redirectTo: '/'
        });

        $locationProvider.html5Mode(true);
    });
```
