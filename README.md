# Angular Infinite Scroll

***

## Usage

### Requirements

* **AngularJS v1.0.0+** is currently required.
* does not require jquery

## Quick start
+ Include the required libraries (cdn/local)

>
``` html
<script src="//ajax.googleapis.com/ajax/libs/angularjs/1.0.5/angular.min.js"></script>
```
+ Include the infinite-scroll js

>
``` html
<script src="infinite-scroll.js"></script>
```

+ Inject the `infinite-scroll` directive into your app module

>
```javascript
angular.module('myApp', ['infiniteScroll']);
```

>
``` html
    <div infinite-scroll="addItems()" threshold="100" can-load="myBoolean"></div>
```

Required Attributes
--------
**infinite-scroll**

The *infinite-scroll* attribute defines the method to call to add items when the scrolling threshold is reached.

Optional Attributes
-------
**threshold**

The *threshold* attribute defines the distance in pixels from the bottom of the content to call the infinite-scroll method when the content is scrolled.

**can-load**

The *can-load* attribute is considered a boolean and controls whether calls to the method defined in *infinite-scroll* should be called when the content is scrolled.

