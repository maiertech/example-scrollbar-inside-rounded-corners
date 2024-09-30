# scrollbar-inside-rounded-corners

## Challenge

On the `main` branch, I have created a simple book list with rounded corners. However, the scrollbar
extends through the rounded corners. How would you fix this?

## Solution

Keep the list height-constrained but add a wrapper. Move the border to the wrapper and set
`overflow: hidden`. Then let the child list scroll.
