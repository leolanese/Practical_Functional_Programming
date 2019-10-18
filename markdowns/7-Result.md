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
function fooSum(a) {
  return b => c => d => e => a + b + c + d + e;
}
fooSum(1)(2)(3)(4)(5); // 15
```
- n. The curried function has two unusual capabilities. First, its arguments needn't be provided one at a time. If f is a ternary function and g is R.curry(f)


```javasript
// we can create a function to curry it: [Ramda - CUrry](https://ramdajs.com/docs/#curry)
const addFourNumbers = (a, b, c, d, e) => a + b + c + d + e;

const curriedAddFourNumbers = R.curry(addFourNumbers);
const f = curriedAddFourNumbers(1, 2);
const g = f(3);
const h = g(4);
h(5); //=> 15
```

- Good points about this approach: The 'R' will encapsulate the source and we don't need to send all the parameters

