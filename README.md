# CSS Flexbox 'space-between' Issue with Oversized Items

This repository demonstrates an uncommon issue related to the `space-between` distribution property in CSS Flexbox.  The issue occurs when the combined width of flex items exceeds the width of their container.  Some browsers handle this situation inconsistently, leading to unexpected layout results.

The `bug.css` file contains the problematic CSS code, and `bugSolution.css` provides a solution.

## Bug

The bug arises from using `justify-content: space-between` when the sum of the widths of flex items is greater than the container's width.  The expected behavior is for items to be distributed evenly, with equal spacing between them, but some browsers may render them incorrectly. 

## Solution

The solution addresses the issue by ensuring the container's width can accommodate all items without causing overflow or unexpected spacing. It leverages different techniques to overcome this limitation.  The provided solution offers more robust and consistent behavior across browsers.