#### QUESTION 10)

#### AC
Combine these multiple Arrays, get the number elements, multiply those by 2

```javascript
const a = ["This", "is", 1, 2, 0];
const b = [true, NaN, -1, "javaScript", 3];
const calc = x => x => x * 2;

[...a, ...b]
  .filter(a => typeof(a) === 'number')
  .map(calc()); // [2, 4, 0, NaN, -2, 6]
```
