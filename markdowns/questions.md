# Practical Functional Programming

## ACTION PLAN
After completing the [Functional (Programming) mindset](https://github.com/leolanese/Becoming-Functional/blob/master/README.md), have a look at the [Functional Programming Keynote](https://github.com/leolanese/Functional-Programming-Keynotes) and follow the action plan from: [Becoming functional](https://github.com/leolanese/Becoming-Functional/blob/master/README.md) to create the following code exercises:

----

### QUESTION 1)

#### AC:
Square all the numbers in an array: 

<details><summary>Results</summary>
<p>
   
```javascript
var arr = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9];

arr.forEach(function(element, index, array){
    array[index] = element* element;
});
console.log(arr); // [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]

```
[Code](https://playcode.io/463485?tabs=1-Result.js.js,preview,console)


</p>
</details>

----

### QUESTION 2)

#### AC:
Sort the following array

<details><summary>Results</summary>
<p>

```javascript
var arr = [0, 1, 5, 3, 4, 2, 9, 7, 8, 6];

var sortDesc = arr => {
    return arr.sort(
       (a, b) => b - a
    );
}; // [9, 8, 7, 6, 5, 4, 3, 2, 1, 0]
```

</p>
</details>

----

### QUESTION 3)

#### AC:
Add or modify the following properties to an Object:
  
```javascript
{ 
  state.brand = 'AUDI';
  state.color = 'Tango Red';
  state.engine = 'V8';
}
```

<details><summary>Results</summary>
<p>

```javascript
const state = {
  brand: 'BMW',
  color: 'Blue',
  extras: ['interior leather', 'cristal roof', 'parking assistance', 'navigation']
};

state.brand = 'AUDI';
state.color = 'Tango Red';
state.engine = 'V8';
```

</p>
</details>

----

### QUESTION 4)

#### AC:
Removing the following  'brand' Object property from the Object:

```javascript
const state = {
  brand: 'BMW',
  color: 'Blue',
  extras: ['interior leather', 'cristal roof', 'parking assistance', 'navigation'],
};
```

<details><summary>Results</summary>
<p>

```javascript
const state = {
  brand: 'BMW',
  color: 'Blue',
  extras: ['interior leather', 'cristal roof', 'parking assistance', 'navigation'],
};
delete state.brand; // true
```

</p>
</details>

----

#### QUESTION 5)

#### AC:
Count the duplicate value inside an array

<details><summary>Results</summary>
<p>

```javascript
var inventory = ['popsicle', 'underwear', 'sauce', 'pens', 'potatoes', 'sauce', 'onion', 'onion', 'pens', 'potatoes', 'ukulele', 'tomahawk', 'underwear', 'popsicle', 'sauce', 'ukulele', 'onion', 'underwear', 'popsicle', 'potatoes', 'onion', 'pens', 'ukulele'];
var count = {};
  
function countItems() {
  inventory.forEach(function(i) { 
    count[i] = (count[i]||0) + 1; 
  });
  console.log(count);
}
```

</p>
</details>

----

#### QUESTION 6)

#### AC:
Replace an item from an Array of Objects where: {a === 3}

<details><summary>Results</summary>
<p>

```javascript
let arr = [ {'a':1,'b':2}, {'a':3,'b':4}, {'a':5,'b':6} ];

index = arr.findIndex(x => x.a === 3); // 1
beforeItems = arr.slice(0, index);
afterItems = arr.slice(index + 1);
newArr = [...beforeItems, {a:666, b:666} , ...afterItems]
```

</p>
</details>

----

#### QUESTION 7)

#### AC:
Sum of all 4 or more parameters paramenters

<details><summary>Results</summary>
<p>

```javascript
function sum(){
  var sum =0; 
  for(var i=0;i<arguments.length;i++){
     sum += arguments[i];
  }
   return sum;
}; // 6
```

</p>
</details>

----

#### QUESTION 8)

#### AC:
Leo Fibonnaci number of 15

<details><summary>Results</summary>
<p>

```javascript
function fib(n) {
  if (n <= 1) {
    return n;
  } else {
    return fib(n - 1) + fib(n - 2);
  }
}

fib(15); // 610
```

</p>
</details>

----

#### QUESTION 9)

#### AC
Remove duplicate elements from array 

<details><summary>Results</summary>
<p>

```javascript
var names = ["Sam", "Carley", "Leo", "Tom", "Leo", "Leo"];

var uniqueArray = function(arrArg) {
  return arrArg.filter(function(elem, pos,arr) {
    return arr.indexOf(elem) == pos;
  });
};
uniqueArray(names); // ["Sam", "Carley", "Leo", "Tom"]
```

</p>
</details>

----

#### QUESTION 10)

#### AC
Combine these multiple Arrays, get the number elements, multiply those by 2

<details><summary>Results</summary>
<p>

```javascript
var a = ["This", "is", 1, 2, 0];
vat b = [true, NaN, -1, "javaScript", 3];

const combined = a.concat(b);

combined
  .filter(a => typeof(a) === 'number')
  .map(x => x * 2); // [2, 4, 0, NaN, -2, 6]
```  

</p>
</details>


