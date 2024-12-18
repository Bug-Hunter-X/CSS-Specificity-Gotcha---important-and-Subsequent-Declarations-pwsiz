# CSS Specificity and !important: Unexpected Behavior

This repository demonstrates a subtle CSS issue involving specificity and the `!important` flag.  The unexpected behavior occurs when an `!important` rule is applied to one property within a selector, and subsequent declarations are made for other properties within the same selector.  This can lead to the browser ignoring the later declarations in certain cases, despite their apparent higher precedence.

The example CSS highlights this issue, demonstrating a scenario where `color: blue;` might not be applied as expected.

**To reproduce:** Open `bug.css` and examine the CSS.  Observe that although the `color` rule is defined, it might not apply correctly in some browsers.

**Solution:**  See `bugSolution.css` for a way to resolve this.