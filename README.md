# CSS Specificity Issue with :hover Pseudo-class

This repository demonstrates a subtle CSS specificity issue related to the `:hover` pseudo-class.  The problem arises when a more specific selector unintentionally overrides a more general selector, leading to unexpected behavior when hovering over parent elements.

## The Problem
The provided CSS code includes two `:hover` rules.  Intentionally, hovering over the container should change the container's background color. Hovering over the link should change the link's color. However, due to CSS specificity rules, only the link's color changes. The container's hover effect is unexpectedly overridden.

## Solution
The solution involves understanding and addressing CSS specificity.  In this case, adjusting the order of the CSS rules or using the `!important` flag (generally discouraged) can resolve the issue. The solution file demonstrates a corrected approach.

## How to Reproduce
1. Clone this repository.
2. Open `bug.html` in a web browser. 
3. Hover over the container and the link. Observe the unexpected behavior.
4. Open `bugSolution.html`.  Observe that the hover effects now work correctly. 

## Conclusion
This example highlights the importance of understanding CSS specificity, especially when working with pseudo-classes like `:hover`.  Careful consideration of selector specificity is crucial for predictable and reliable CSS behavior. 