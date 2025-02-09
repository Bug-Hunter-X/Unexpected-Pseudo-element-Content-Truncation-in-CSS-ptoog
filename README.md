# Unexpected Pseudo-element Content Truncation

This repository demonstrates an uncommon CSS bug where a pseudo-element's content gets unexpectedly truncated when using `word-break: break-all;` and `overflow: hidden;` on its parent container.  The bug is subtle and might not occur consistently across all browsers.

## Bug Description

The `bug.css` file contains CSS code that reproduces the issue. A long string set as the content of a `::before` pseudo-element is unexpectedly cut off due to the interaction between `word-break: break-all;` and `overflow: hidden;` on the parent.

## Solution

The `bugSolution.css` file offers a possible solution by using `text-overflow: ellipsis;` to gracefully handle overflowing text instead of relying on `overflow: hidden;` alone.  This provides a visually better way to truncate text.

## Contributing

Contributions are welcome! Feel free to open issues and pull requests to improve this example or report similar edge-case scenarios.