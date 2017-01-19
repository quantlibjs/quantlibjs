# QuantLib in Pure JavaScript [![npm version](https://badge.fury.io/js/quantlib.js.svg)](http://badge.fury.io/js/quantlib.js) [![Bower version](https://badge.fury.io/bo/quantlib.js.svg)](https://badge.fury.io/bo/qunatlib.js) [![Twitter Follow](https://img.shields.io/twitter/follow/quantlibjs.svg?style=social&maxAge=3600)](https://twitter.com/quantlibjs)


> This project is still at very early stage, **DO Expect Bugs**

> Template classes, enumerations will be added for later

## Getting started

```sh
npm install quantlib.js
```

or

```sh
bower install quantlib.js
```

### Usage

#### Load the library

* Browser

`$ql will be created after loading js file

* Node.js

var $ql = require('quantlib.js');

#### Class

class names are same as [QuantLib](http://quantlib.org/) project.

use `new` to create object

```js
// create a new Matrix object
var m1 = new $ql.Matrix({
                          "rows:6",
                          "columns":9
                        });
```

```sh
> m1
Matrix { ptr: 13611328 }
> m1.rows();
6
> m1.columns();
9
```

#### Function Overloading

Function names are same as QuantLib, and all functions takes one parameter: `opts`

If function has no paramter, just call it without paramter, otherwise pass a `JSON` object to the function, in this object put `paramter: value` elements, the paramter name must match QuantLib functions.
