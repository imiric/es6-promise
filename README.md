# ES6-Promises

This is a polyfill of
[ES6 Promises](https://github.com/domenic/promises-unwrapping). The implementation
is basically an API remapping of [rsvp.js](https://github.com/tildeio/rsvp.js).

For API details and how to use promises, see the
[JavaScript Promises HTML5Rocks article](http://www.html5rocks.com/en/tutorials/es6/promises/).

This repo is a [component(1)](http://component.io) wrapper around the work
@jakearchibald did at the
[original repo](https://github.com/jakearchibald/es6-promise). All credit goes
out to him.

## Installation

  Install with [component(1)](http://component.io):

    $ component install imiric/es6-promise

## API

```js
var promise = require('es6-promise');
promise.polyfill();  // setup polyfill or fallback to native implementation
// use as per the spec
var p = new Promise(function(resolve, reject) {
  // do a thing, possibly async, then...

  if (/* everything turned out fine */) {
    resolve("Stuff worked!");
  }
  else {
    reject(Error("It broke"));
  }
});
```

## License

  [MIT](LICENSE)
