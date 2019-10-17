### QUESTION 3)

### AC
Add or modify the following properties to an Object:

```javascript
const state = {
  brand: 'BMW',
  color: 'Blue',
  extras: ['interior leather', 'cristal roof', 'parking assistance', 'navigation'],
};

const newState = {
  ...state,
  brand: 'AUDI',
  color: 'Tango Red',
  engine: 'V8',
}

/*
{
  brand: "AUDI"
  color: "Tango Red"
  engine: "V8"
  extras: ["interior leather", "cristal roof", "parking assistance", "navigation"]
}
*/
```

- we're spreading the key-value pairs of the original object onto a new one
