Nordic.js notes 2014
=========

Notes from Nordic.js 2014

## Crockford - The Better parts
Douggie shed his thoughts on the coming ES6 specification and stirred some feelings with an incensitive remark about masculine code - which he corrected until evening. Douggies new favorite new parts are:
* proper tail recursion
* let - function scope
* ..rest - parameter
* destructuring
* weakMaps
 
```js
function doWhile(condition) {
  var result = performTask(condition);
  if (result !== undefined) {
    doWhile(result);
  }
}
```

Then came the bad parts...
"The worst new feature in ES6 is class, most requested by java developers who don't want to learn JavaScript. Those people will go to their grave never knowing how miserable they are."
 
Go figure.
 
- Stopped using New Years ago
- Stopped using Object.create
- Stopped using this
- Stopped using Null
- Stopped using falsiness
- Stopped using for
- Will stop using while & do
 
Class free programming
```js
function constructor(spec) {
  let {member} = spec,
      {other} = other_constructor(spec);,
      method = function() {
        // member, other, method, spec
      };
 
  return Object.freeze({
    meyhod,
    other
  });
}
```

## Tom Dale

Gave an introduction to web components Ember style and some live coding that actually worked!
