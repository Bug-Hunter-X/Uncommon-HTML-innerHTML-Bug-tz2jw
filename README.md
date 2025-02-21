# Uncommon HTML innerHTML Bug

This repository demonstrates an uncommon bug related to setting the `innerHTML` property of an HTML element using multiple lines.  The issue arises when attempting to build the `innerHTML` incrementally, line by line. Only the last line assigned will be rendered in the final output.

This is a subtle error that can easily be overlooked. The solution involves properly concatenating the HTML strings before assigning them to the `innerHTML` property. 

## How to Reproduce the Bug

1. Open `bug.html` in a web browser.
2. Observe that only "Line 3" is displayed in the div.

## Solution

The solution involves concatenating the HTML strings before setting the `innerHTML`. The corrected code can be found in `bugSolution.html`.