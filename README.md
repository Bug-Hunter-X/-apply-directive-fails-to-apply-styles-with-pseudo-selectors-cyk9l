# Tailwind CSS @apply Directive Bug with Pseudo-selectors

This repository demonstrates a bug where Tailwind CSS's `@apply` directive fails to apply styles when used with pseudo-selectors like `:hover` and `:focus`.  The issue stems from how `@apply` handles the merging of styles and the specificity of pseudo-class selectors.

## Reproduction Steps

1. Clone this repository.
2. Open `bug.html` in your browser.
3. Observe that the hover effect on the button does not work as expected.
4. Open `bugSolution.html` to see the corrected implementation.

## Solution

The solution involves avoiding the use of `@apply` with pseudo-selectors. Instead, directly apply the classes to the element using the standard class attribute.  This ensures correct style application, including pseudo-selector styles.