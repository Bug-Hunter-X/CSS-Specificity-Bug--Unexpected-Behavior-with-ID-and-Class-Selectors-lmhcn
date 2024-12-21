# CSS Specificity Bug

This repository demonstrates an uncommon bug related to CSS specificity.  The issue arises when combining ID and class selectors with the same element, resulting in unexpected behavior.  The most specific selector does not override previous selectors due to how CSS specificity rules work.

## Bug Description

The bug is demonstrated in `bug.css`.  Despite using a more specific selector (`#myElement.myElement`), the color of the element remains blue (defined by `#myElement`) rather than green (defined by `#myElement.myElement`).

## Solution

The solution, found in `bugSolution.css`, involves restructuring the CSS to ensure the intended styling is applied correctly using appropriate specificity. 

## How to Reproduce

1. Clone the repository.
2. Open `bug.html` in a web browser.
3. Observe that the text is blue instead of green.
4. Open `bugSolution.html` in a web browser.
5. Observe that the text is correctly styled as green.