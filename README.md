Baasic AngularJS -1.x Article Module Hello World represented by Angularjstutorials.net
============

In order to create a hello world sample based on the Baasic article module you need follow the below steps below:

# Create AngularJS hello world application

# Include AngularJS as below

You have to include the downloaded JavaScript file (angular.min.js) in the HTML document to use angularJS.

The belwo HTML shows how to include angular.min.js.

```html
<!doctype html>
<html>
   <head>
       <script type="text/javascript" src="angular.min.js"></script>
   </head>
   <body>
   </body>
</html>

```
You can also use the CDN but make sure to check with the angularJS website for the latest version.

```html
<!doctype html>
<html>
   <head>
       <script type="text/javascript" src="https://ajax.googleapis.com/ajax/libs/angularjs/1.2.26/angular.min.js"></script>
   </head>
   <body>
   </body>
</html>

```

# AngularJS 1.x Hello World Example

Now we are going to write our first AngularJS application. We have gone through the following steps to create our first Angular application:

1. First step is to Include angularJS file in the HTML document. You can use angular.min.js or the CDN.
2. Second step is to indicate the active portion of angular application. The directive ng-app   tells the Angular which part of our document belongs to the angular application.
3. The directive ng-model and ng-bind is to bind the input text value to the specified HTML
element. We will explain these concepts in the coming posts. For now, just say hello to your first angular application.

```html
<!DOCTYPE html>
<html lang="en">
<title>AngularJS First Application</title>

<head>
    <script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.2.26/angular.min.js"></script>
</head>

<body>
<div ng-app>

   <p>Enter Some text : <input type="text" ng-model="someText"></p>
   <p>Hello <span ng-bind="someText"></span>!</p>

</div>
</body>
</html>

```

The ng-bind directive tells Angular to replace the text of the element with the given value , and  it is updated  with change in the value of that expression.

Typically, we do not use the ng-bind directive directly in our document. We wrap the model value in double curly braces like {{some-expression}}. The following example demonstrates how the model value is wrapped inside the double curly braces. You will see the same result in your browser.


```html
<!DOCTYPE html>
<html lang="en">
<title>AngularJS First Application</title>

<head>
    <script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.2.26/angular.min.js"></script>
</head>

<body>
<div ng-app>

   <p>Enter Some text : <input type="text" ng-model="someText"></p>
   <p>Hello {{ someText }}!</p>

</div>
</body>
</html>

```