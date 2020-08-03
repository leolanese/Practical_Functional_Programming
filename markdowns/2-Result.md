### QUESTION 2)

#### AC:
Sort the following array

```javascript
const arr = [0, 1, 5, 3, 4, 2, 9, 7, 8, 6];

[...arr].sort().reverse(); // [9, 8, 7, 6, 5, 4, 3, 2, 1, 0]
```

- sort() is a [mutator method](https://www.educative.io/edpresso/javascript-mutator-methods) and it cause a 
side-effect, we need to adopt spread, we can make a copy of the array so the mutation happends on the copy, instead the original array.

