# Tailwind CSS @apply Directive Inconsistency Within Custom Directives

This repository demonstrates a bug where Tailwind CSS's `@apply` directive, when used inside a custom directive, may fail to apply styles correctly.

## Bug Description

The issue manifests as unexpected visual inconsistencies in elements where a custom directive containing `@apply` is used. Styles applied using `@apply` might not be reflected in the rendered output, leading to styling problems.

## Reproduction

1. Clone this repository.
2. Run your build process for Tailwind CSS.
3. Observe the affected elements.  The styles applied via `@apply` within the custom directive will likely be missing.

## Solution

This issue can often be resolved by carefully structuring your custom directives and ensuring that they are properly applied in your main CSS or JavaScript files. Refer to the `bugSolution.css` file for a corrected approach.

## Note

The exact cause of this inconsistency can sometimes be tied to how the CSS is parsed and ordered during the build process. The solution focuses on reliable structural patterns to mitigate the issue.