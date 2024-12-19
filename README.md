# CSS calc() Unexpected Behavior in Nested Elements

This repository demonstrates a common issue with the CSS `calc()` function when used in nested elements. The problem arises when the parent element's dimensions are not explicitly defined or are dynamically affected by other CSS rules, causing incorrect calculations within the nested element.

The `bug.css` file contains the problematic code, while `bugSolution.css` provides a corrected version.

## Steps to reproduce:

1. Clone the repository.
2. Open `index.html` (you may need to create a simple HTML structure to see the effect). 
3. Observe the layout difference between the two sections with the original and fixed code.

## Solution:

The issue is resolved by explicitly setting the width (or height) of the parent element.  This gives the `calc()` function a solid baseline to work with, ensuring the calculation produces the expected result.  If the parent's dimensions are dynamic, ensure to manage those dependencies to guarantee calculation accuracy.