#### QUESTION 6)

#### AC:
Replace an item from an Array of Objects where: {a === 3}

```javascript
const arr = [ {'a':1,'b':2}, {'a':3,'b':4}, {'a':5,'b':6} ];
[...arr.slice(0,index), {'x':666}, ...arr.slice(index + 1, arr.length)]; //  [{a: 1, b: 2},{a: 666, b: 666},{a: 5, b: 6}]
```
