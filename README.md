# Uncommon HTML Error: Incorrect innerHTML Usage

This repository demonstrates an uncommon error related to the use of `innerHTML` in HTML.  The error arises from assigning a non-string value (a number in this example) to the `innerHTML` property of an HTML element.  This can lead to unexpected behavior or silent failures, making it harder to debug.

## The Bug
The `bug.html` file contains a simple HTML structure with a div element and a JavaScript script. The script attempts to set the `innerHTML` of the div to a number (123). This is incorrect; `innerHTML` expects a string.

## The Solution
The `bugSolution.html` file shows the corrected version.  The number is converted to a string using `String()` before being assigned to `innerHTML`. This ensures that the browser correctly interprets the value and renders the content.