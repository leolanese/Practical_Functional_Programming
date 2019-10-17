#### QUESTION 7)

#### AC:
Sum of all 4 or more parameters parameters

```javascript
// using spread operator
function sum(...args) {
  return args.reduce((previous, current) => {
    return previous + current;
  });
}
console.log(sum(1, 2, 3, 4));
```

- Using Functions Rest Parameters, one of the objectives is sending all the parameters that a function needs instead using a variable from outside scope and mutate. 


```javasript
// using currying
function sum(a) {
  return b => c => d => e => a + b + c + d + e;
}
sum(1)(2)(3)(4)(5);
```
