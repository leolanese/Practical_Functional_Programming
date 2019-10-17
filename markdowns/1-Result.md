### QUESTION 1)

#### AC:
Square all the numbers in an array: 

```javascript
const arr = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9];
arr.map(num => Math.pow(num, 2)); // [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]
```

- Shifting to a functional approach to tackle this same task, you only need to be concerned with applying the right behavior block, like crafting, at each element.
- Compared with the previous example, you see that this code "frees you from the responsibility" of properly managing a loop counter and array index access, in other words, we are abstracting blocks of logic that will simplify the code: The more code you have, the more chances to produce bugs.
- Why remove loops from your code? A loop is an Imperative Control Structure that is hard to reuse, also and difficult to plug in to other operations. In addition, it implies code that's constantly changing or mutating in response to new iterations.
