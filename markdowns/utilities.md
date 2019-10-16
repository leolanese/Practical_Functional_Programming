// Currying is a transform that makes f(a,b,c) callable as f(a)(b)(c).
```javascript
const curry = (f, ...args) => (f.length <= args.length) ?
    f(...args) :
    (...more) => curry(f, ...args, ...more);
```

// const compose = (f, g) => (a) => f(g(a)) 
```javascript
const compose  = (fn, ...rest) =>
  rest.length === 0 ?
    fn :
    (...args) => fn(compose(...rest)(...args));
```



