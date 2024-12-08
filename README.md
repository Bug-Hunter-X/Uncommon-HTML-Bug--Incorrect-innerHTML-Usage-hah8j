# Uncommon HTML Bug: Incorrect innerHTML Usage

This repository demonstrates a subtle bug related to the usage of `innerHTML` in HTML.  The bug stems from how `innerHTML` handles and replaces existing content within an HTML element.  Improper use can lead to unexpected behavior and, in certain scenarios, create security vulnerabilities such as cross-site scripting (XSS) if not handled carefully.  This example is to show how it should be done to avoid future bugs.

## Bug Description

The code contains a scenario where `innerHTML` is used to replace the content of a div element. The issue is that the replacement text is not completely replacing the initial content, leading to unexpected behavior and making it not user friendly.

## Bug Solution

The solution involves making sure that the `innerHTML` replacement completely replaces the initial content and avoid potential vulnerabilities by sanitizing user inputs before using them to update the `innerHTML` property.

## How to Reproduce

1. Clone this repository.
2. Open `bug.html` in your web browser. Observe the unexpected behavior.
3. Open `bugSolution.html` to see the corrected version. 