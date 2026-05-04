# Part 1 Answers

## Q1
Line 9 prints: `values added: 20`.

This happens because `var` has function scope, so a variable declared inside an `if` block can still be accessed elsewhere inside the same function.

## Q2
Line 13 prints: `final result: 20`.

This happens because `result` was declared using `var`, so it is accessible throughout the whole function.

## Q3
You should avoid using `var` because it has function scope instead of block scope. This can make variables accessible in places where the programmer may not expect them to be accessible, which can cause bugs and naming conflicts.

## Q4
Line 9 prints: `values added: 20`.

This happens because `let` is accessible inside the block where it is declared.

## Q5
Line 13 causes a `ReferenceError`.

This happens because `result` was declared using `let` inside the `if` block, so it cannot be accessed outside that block.

## Q6
Line 9 prints: `values added: 20`.

This happens because `const` is accessible inside the block where it is declared.

## Q7
Line 13 causes a `ReferenceError`.

This happens because `const` has block scope, just like `let`, so `result` cannot be accessed outside the block where it was declared.