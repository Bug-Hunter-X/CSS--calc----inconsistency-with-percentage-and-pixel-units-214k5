# CSS `calc()` Inconsistency Bug

This repository demonstrates a common issue with the CSS `calc()` function when combining percentage and fixed-unit values (e.g., pixels).  The problem arises from the order of operations and how different browsers might interpret the calculation, especially when the parent element's dimensions are not precisely specified.

## Bug Description
The `calc()` function in CSS allows dynamic calculations of lengths.  However, when percentages are used in conjunction with pixel values (or other units) the results can be inconsistent across browsers. This is often due to the browser calculating the percentage before the pixel subtraction, leading to unexpected results.

## How to Reproduce
1. Clone this repository.
2. Open `bug.html` in different browsers (Chrome, Firefox, Safari, etc.).
3. Observe the different widths of the element.  The inconsistency in width demonstrates the problem.