#### QUESTION 9

#### AC
Remove duplicate elements from array 

```javascript
// using reduce & spread
const array = ["Sam", "Carley", "Leo", "Tom", "Leo", "Leo"];
array.reduce((unique, item) => unique.includes(item) ? unique : [ ...unique, item], []); // ["Sam", "Carley", "Leo", "Tom"]
```

```javascript
// using filter & indexOf
const array = ["Sam", "Carley", "Leo", "Tom", "Leo", "Leo"];
array.filter((item, index) => array.indexOf(item) === index); // ["Sam", "Carley", "Leo", "Tom"]
```


```javascript
// using spread & Set
const names = ["Sam", "Carley", "Leo", "Tom", "Leo", "Leo"];
console.log([...new Set(names)]); // ["Sam", "Carley", "Leo", "Tom"]
```
- Set is a new data object introduced in ES6. Because Set only lets you store unique values. 
When you pass in an array, it will remove any duplicate values.
