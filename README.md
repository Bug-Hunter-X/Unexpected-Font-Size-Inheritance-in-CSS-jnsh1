# Unexpected Font Size Inheritance in CSS

This repository demonstrates an uncommon CSS bug related to specificity and inheritance.  A paragraph element inside a container unexpectedly inherits the font size from a more specific div selector, even though it has no explicit font size set.

## Problem

The `p` element inherits the `font-size` from the `div` inside the `.container`, not from the global `div` selector or any specific rule on paragraph elements inside `.container` itself. This might not always be immediately clear and could be difficult to track down in larger projects. This is mainly due to inheritance behavior of CSS. 

## Solution

The solution involves being explicit about the font size for the `p` element within the `.container` to override the inherited style from the more specific `div` selector.

The solution is provided in the `bugSolution.css` file.