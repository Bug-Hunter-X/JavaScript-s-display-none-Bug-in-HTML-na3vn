# Uncommon HTML Bug: display: none JavaScript Issue

This repository demonstrates a subtle bug related to using `display: none` in JavaScript within HTML.  The bug arises from the fact that setting `display: none` on an element can interfere with subsequent attempts to modify its visual properties using JavaScript.

The `bug.html` file showcases the problem.  The `solution.html` provides a corrected version.

## Bug Description

The core issue lies in the sequence of operations:

1. An HTML element's display property is set to `none` using JavaScript.
2. After a delay, an attempt is made to change the display property (e.g., to `block`) to make the element visible again.

The incorrect usage of display:none in JavaScript results in the element remaining hidden even after attempting to alter the property. The solution illustrates how to correctly address this issue.

## Solution

The provided solution correctly manipulates the element's display property without causing the interference exhibited by the bug.  It offers a robust alternative that ensures the expected behavior.  The key is avoiding the use of display:none in a manner that prevents subsequent style manipulation.
