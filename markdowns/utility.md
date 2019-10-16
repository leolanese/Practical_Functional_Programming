// Currying is a transform that makes f(a,b,c) callable as f(a)(b)(c).
```javascript
// https://javascript.info/currying-partials
function curried(...args) {
  if (args.length >= func.length) { // (1)
    return func.apply(this, args);
  } else {
    return function pass(...args2) { // (2)
      return curried.apply(this, args.concat(args2));
    }
  }
};
```


