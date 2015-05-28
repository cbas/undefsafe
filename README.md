undefsafe
=========

Simple *function* for retrieving deep object properties without getting "Cannot read property 'X' of undefined"

## Usage

```js
var object = {
  a: {
    b: {
      c: 1,
      d: [1,2,3],
      e: 'remy'
    }
  }
};

console.log(undefsafe(object, 'a.b.e')); // "remy"
console.log(undefsafe(object, 'a.b.not.found')); // undefined
```

Demo: [https://jsbin.com/eroqame/3/edit?js,console](https://jsbin.com/eroqame/3/edit?js,console)
