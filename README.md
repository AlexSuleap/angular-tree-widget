Agular Tree Widget
================

Light [AngularJS](http://www.angularjs.org) tree widget control, without jQuery dependency.

![ScreenShot](https://github.com/AlexSuleap/angular-tree-widget/blob/master/demo/img/demo.png)

## Features

- Reacts at model changes.
- Isolated scope.
- Easy customizable using css.
- Custom icons[or no icons at all].
- Multiple selection.
- Disabled nodes.

## Demo

Watch the tree in action on the [demo page](http://alexsuleap.github.io/).

## Instalation

1. [Download](/AlexSuleap/angular-tree-widget/archive/master.zip) the project.
2. Load the style and the script in your project:

```html
<script type="text/javascript" src="/angular-tree-widget.min.js"></script>
<link rel="stylesheet" type="text/css" href="/angular-tree-widget.min.css">
```
3. Add a dependency to your application module.

```javascript
angular.module('myApp', ['TreeWidget']);
```
4. Add data for the tree
```javascript	
$scope.treeNodes =[{
	name: "Node 1",
        children: [{
            name: "Node 1.1",
            children:[
				{name:"Node 1.1.1"},
				{name: "Node 1.1.2"}]
        }]
	},{
        name: "Node 2",
        children: [
			{name: "Node 2.1"},
			{name: "Node 2.2"}
		]
    }];
```
5. Add the tree tag to your application.
```html
<tree nodes='treeNodes'>
```
5. Do not forget to add [AngularJS](http://www.angularjs.org), [AngularJS.Animate](http://www.angularjs.org) and [Angular Recursion](https://github.com/marklagendijk/angular-recursion) references to your project.