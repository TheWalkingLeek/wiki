## Synonym to .map

```
numbers = [1,5,6,16]
are_numbers_even = numbers.collect do |number|
if number % 2 == 0
   return true
else
   return false
end

--> are_numbers_even = [false, false, true, true]
```

iterates like a foreach loop but returns an array. In the block of your loop, with all your statements in it, you return a value that's written inside the returning array