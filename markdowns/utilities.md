// Currying is a transform that makes f(a,b,c) callable as f(a)(b)(c).
```javascript
const curry = (f, ...args) => (f.length <= args.length) ?
    f(...args) :
    (...more) => curry(f, ...args, ...more);
```


// const compose = (f, g) => (a) => f(g(a)) = a . g .f 
```javascript
const compose = (...functions) => args => functions.reduceRight((arg, fn) => fn(arg), args);
```

// const compose = (f, g) => (a) => f(g(a)) = f . g .a
```javasccript
const pipe = (...functions) => args => functions.reduce((arg, fn) => fn(arg), args);
```
