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