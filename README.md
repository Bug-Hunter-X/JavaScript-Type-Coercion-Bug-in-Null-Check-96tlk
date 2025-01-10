# JavaScript Type Coercion Bug

This repository demonstrates a subtle bug in JavaScript related to type coercion and null checks. The `foo` function aims to return `null` if either input `a` or `b` is `null`. However, due to JavaScript's loose typing, the function might produce unexpected results when dealing with falsy values such as 0, "", or false. 

## Bug Description
The function uses strict equality (`===`) for null checks. While this is generally good practice, it doesn't handle the case where a falsy value other than null is passed.  This results in unintended behavior.

## Solution
The solution addresses this by explicitly checking for null and undefined using a stricter conditional or utilizing optional chaining and nullish coalescing.

## How to Run
1. Clone this repository.
2. Open `bug.js` and `bugSolution.js` in a code editor or IDE.
3. Run the JavaScript code using Node.js or a browser's developer console to observe the differences in behavior.