#### QUESTION 12)

#### AC
Find a text inside an string


```javascript
const someText = 'javascript rules :)';

console.log(someText.includes('rules')); // true
console.log(['leo', 'JS', someText].includes('leo')); // true
```


```javascript
// using '~' Bitwise
const someText = 'javascript rules :)';

console.log(!!~someText.indexOf('rules')); // true
```
