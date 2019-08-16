## String to number

Even in Javascript, it's sometimes usefull to convert a String to a number (especially in combination with typescript)

```
let x = '1'
+x --> 1
x = 'a'
+x --> NaN
```

## Arrow functions

```
[1,2,3].forEach((x) => {
  console.log(x)
})
```

Has the same **this, arguments, super or new.target** as in the context outside.

## Regular functions

```
[1,2,3].forEach(function(x) {
  console.log(x)
})
```
