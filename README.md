# Uncommon HTML Bug: DOM Manipulation Timing

This repository demonstrates a common, yet sometimes subtle, bug related to the timing of DOM manipulation in JavaScript within HTML.

The `bug.html` file contains the erroneous code. It attempts to add an event listener to a div element before the DOM is fully loaded. This frequently results in a runtime error because the element doesn't yet exist when the script runs.

The `bugSolution.html` file provides a corrected version. It leverages the DOMContentLoaded event to guarantee the script runs only after the DOM is fully parsed and ready.

## How to Reproduce

1. Clone this repository.
2. Open `bug.html` in a web browser.  You'll likely encounter an error in the browser's developer console.
3. Open `bugSolution.html`. This version should work correctly.