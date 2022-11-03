#BigO

**Big O Notation** is a way of describing the relationship between the input to a function or as it grows and how that changes the runtime of that function, the relatinship between the input size and the time relative to that input.

We say that an algorithm is O(f(n))) if the number of simple operations the computer has to do is eventually less than a constant times f(n), as n increases

f(n) could be:

- linear (f(n) = n)
- quadratic (f(n) = n(power2))
- constant (f(n) = 1 )
- something entirely different
  <sub>f(n) - operation
  n - time</sub>

  Examples:

**O(1)**

```javascript
function sumOfIntegers(n) {
  return (n * (n + 1)) / 2;
}
```

3 operations[* + /] => O(1)

**O(n)**

```javascript
function sumOfIntegers(n) {
  let total = 0;
  for (let i = 1; i <= n; i++) {
    total += i;
  }
  return total;
}
```

Number of operations is (eventually) bounded by multiple a of n
[i++, total+=, loop] => O(n)

**O(n²)**

```javascript
function printPairsOfNumbers(n) {
  for (var i = 0; i < n; i++) {
    for (var j = 0; j < n; j++) {
      console.log(i, j);
    }
  }
}
```

O(n) operation inside O(n) operation [nested loops]

** Space Complexity in JS **

- Most primitives (booleans, numbers, undefined, null) are constant space
- Strings require O(n) space (where n is the string length)
- Reference types are generally O(n), where n is the key length (for arrays) of the number of keys (for objects)
