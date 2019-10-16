----

#### EXAMPLE 7)

#### AC:
Sum of all 4 paramenters

```javascript
function sum(...args) {
  return args.reduce((previous, current) => {
    return previous + current;
  });
}
console.log(sum(1, 2, 3, 4));
```

- Using Functions Rest Parameters, one of the objectives is sending all the parameters that a function needs instead using a variable from outside 
scope and mutate. 

