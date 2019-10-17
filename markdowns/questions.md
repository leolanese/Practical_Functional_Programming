# Practical Functional Programming

## ACTION PLAN
After completing the (Functional (Programming) mindset)[https://github.com/leolanese/Becoming-Functional/blob/master/README.md], have a look at the (Functional Programming Keynote)[https://github.com/leolanese/Functional-Programming-Keynotes] and follow the action plan from: (Becoming functional)[https://github.com/leolanese/Becoming-Functional/blob/master/README.md] to refactor the following code exercises:

----

### QUESTION 1)

#### AC:
Square all the numbers in an array: 

```javascript
var arr = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9];

for(let i = 0; i < arr.length; i++) {
   arr[i] = Math.pow(arr[i], 2);
}
array; // [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]
```


----

### QUESTION 2)

#### AC:
Sort the following array

```javascript
var arr = [0, 1, 5, 3, 4, 2, 9, 7, 8, 6];

var sortDesc = arr => {
    return arr.sort(
       (a, b) => b - a
    );
}; // [9, 8, 7, 6, 5, 4, 3, 2, 1, 0]
```


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
delete state.brand; // true
```

----

#### QUESTION 5)

#### AC:
Count the duplicate value inside an array

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

----

#### QUESTION 6)

#### AC:
Replace an item from an Array of Objects where: {a === 3}

```javascript
let arr = [ {'a':1,'b':2}, {'a':3,'b':4}, {'a':5,'b':6} ];

index = arr.findIndex(x => x.a === 3); // 1
beforeItems = arr.slice(0, index);
afterItems = arr.slice(index + 1);
newArr = [...beforeItems, {a:666, b:666} , ...afterItems]
```

----

#### QUESTION 7)

#### AC:
Sum of all 4 or more parameters paramenters

```javascript
function addFourNumbers(a, b, c, d) {
  return a + b + c + d
}
addFourNumbers(1,2,3,4); // 10
```

----

#### QUESTION 8)

#### AC:
Leo Fibonnaci number of 15

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

