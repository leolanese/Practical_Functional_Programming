#### EXAMPLE 8)

#### AC:
Leo Fibonnaci number of 15

```javascrcipt
const fib = x => (x === 0 || x === 1 )
                 ? x
		             : fib(x-1) + fib(x-2);
fib(15); // 610
```

