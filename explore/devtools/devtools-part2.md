# DevTools Part 2

## Q1
The bug was that `num1` and `num2` were read from the input fields as strings. Because of this, the `+` operator performed string concatenation instead of numeric addition.

## Q2
I would fix it by converting `num1` and `num2` into numbers before adding them.

```js
let result = Number(num1) + Number(num2);