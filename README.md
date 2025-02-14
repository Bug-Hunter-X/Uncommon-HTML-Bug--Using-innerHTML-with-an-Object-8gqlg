# Uncommon HTML Bug: Incorrect innerHTML Usage

This repository demonstrates an uncommon bug related to the usage of `innerHTML` in HTML.  The problem lies in attempting to assign a JavaScript object directly to `innerHTML`, instead of a string. This often leads to unexpected behavior, where nothing renders or an error is thrown, depending on the browser.

## Bug Description
The bug occurs when attempting to directly set the `innerHTML` of an element to a JavaScript object.  `innerHTML` expects a string; passing an object will not work as intended.

## Solution
The solution involves converting the JavaScript object into a string representation before assigning it to `innerHTML`.  This can be done using `JSON.stringify` to get a JSON representation or by manually creating the appropriate string.

## How to Reproduce
1. Clone this repository.
2. Open `bug.html` in your web browser.
3. Observe that the text within the div is not replaced as expected.
4. Open `bugSolution.html` to see the corrected version.