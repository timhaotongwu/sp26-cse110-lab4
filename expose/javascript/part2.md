# Part 2 Answers

## Q1
Line 12 causes a `ReferenceError`.

This happens because `i` is declared using `let` inside the `for` loop, so it only exists inside the loop block and cannot be accessed outside the loop.

## Q2
Line 13 prints: `150`.

This happens because `discountedPrice` is declared using `var`, so it has function scope and can still be accessed outside the loop.

## Q3
Line 14 prints: `150`.

This happens because `finalPrice` is declared using `var`, so it is accessible throughout the function.

## Q4
The function returns `[50, 100, 150]`.

Each original price is multiplied by `(1 - discount)`, then rounded to two decimal places and pushed into the `discounted` array.

## Q5
Line 12 causes a `ReferenceError`.

This happens because `i` is declared with `let` inside the `for` loop, so it cannot be accessed outside the loop.

## Q6
Line 13 causes a `ReferenceError`.

This happens because `discountedPrice` is declared with `let` inside the loop block, so it cannot be accessed outside that block.

## Q7
Line 14 prints: `150`.

This happens because `finalPrice` is declared outside the loop with `let`, so it can still be accessed after the loop finishes.

## Q8
The function returns `[50, 100, 150]`.

Each price is multiplied by `(1 - discount)`. With the call `discountPrices([100, 200, 300], 0.5)`, the discounted prices are 50, 100, and 150.

## Q9
Line 11 causes a ReferenceError.

This happens because i is declared with let inside the for loop, so it only exists inside the loop block and cannot be accessed after the loop.

## Q10
Line 12 prints: 3.

This happens because length is declared with const in the function scope, so it can still be accessed after the loop.

## Q11
The function returns [50, 100, 150].

discounted is a const array, but its contents can still be changed with push(). Each price is multiplied by 0.5 and added to the array.

## Q12

A. Accessing the value of the `name` property:

```js
student.name
```

B. Accessing the value of the `Grad Year` property:

```js
student["Grad Year"]
```

C. Calling the function for the `greeting` property:

```js
student.greeting()
```

D. Accessing the `name` property of the object in the `Favorite Teacher` property:

```js
student["Favorite Teacher"].name
```

E. Accessing index zero in the array of the `courseLoad` property:

```js
student.courseLoad[0]
```

## Q13 Arithmetic

### `'3' + 2`
Output: `"32"`  
Because `+` with a string performs string concatenation.

### `'3' - 2`
Output: `1`  
Because `-` converts `"3"` into the number `3`.

### `3 + null`
Output: `3`  
Because `null` converts to `0`.

### `'3' + null`
Output: `"3null"`  
Because `+` with a string concatenates.

### `true + 3`
Output: `4`  
Because `true` converts to `1`.

### `false + null`
Output: `0`  
Because `false` converts to `0` and `null` converts to `0`.

### `'3' + undefined`
Output: `"3undefined"`  
Because `+` with a string concatenates.

### `'3' - undefined`
Output: `NaN`  
Because `undefined` converts to `NaN`.

## Q14 Comparison

### A. `'2' > 1`
Output: `true`

### B. `'2' < '12'`
Output: `false`

### C. `2 == '2'`
Output: `true`

### D. `2 === '2'`
Output: `false`

### E. `true == 2`
Output: `false`

### F. `true === Boolean(2)`
Output: `true`

## Q15
`==` checks equality after type conversion.
`===` checks strict equality, so both value and type must match.

## Q16

The code is written in part2-question16.js.

The loop iterates through each property in the object and prints the value if the property name starts with "r" or if the value is an odd number.

Output:
21
45
5
2

## Q17

The result is `[2, 4, 6]`.

The function `modifyArray` takes the array `[1, 2, 3]` and the callback function `doSomething`. It loops through each value in the array and applies `doSomething` to it. Since `doSomething(num)` returns `num * 2`, the values become `2`, `4`, and `6`.

## Q18

The code is written in part2-question18.js.

The program uses `setInterval()` to print the current time every 1000 milliseconds, which means it prints the time once every second.

## Q19

The output is:

1
4
3
2

This happens because 1 is printed first. Then the two setTimeout() calls are scheduled, but they do not run immediately. After that, 4 is printed. Even though the timeout for 3 is 0 milliseconds, it still waits until the current call stack finishes, so 3 prints after 4. Finally, 2 prints last because it has a longer delay.