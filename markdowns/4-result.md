----

### EXAMPLE 5)

#### AC:
Removing the following  'brand' Object property from the Object:

```javascript
const state = {
  brand: 'BMW',
  color: 'Blue',
  extras: ['interior leather', 'cristal roof', 'parking assistance', 'navigation'],
};
const { brand, ...newState } = state;
```

- We're usign rest operator using [destructuring assignment](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Destructuring_assignment): 
We assign quantity key-value pair to constant quantity and assign rest of the object to newState.
