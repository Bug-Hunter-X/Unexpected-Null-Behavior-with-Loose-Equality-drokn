# Unexpected Null Behavior with Loose Equality in JavaScript

This repository demonstrates a common JavaScript bug related to loose equality (`==`) and null checks.  The code in `bug.js` uses loose equality to check for null values, which can lead to unexpected behavior when comparing null with other falsy values like 0 or false. The `bugSolution.js` file provides a corrected version of the code that uses strict equality (`===`) to resolve this issue.

## Problem

The original code incorrectly uses loose equality (`==`) to check for `null` values.  This can lead to unexpected results when other falsy values (0, '', false, etc) are passed as arguments.  Loose comparison can be problematic when dealing with different types that might have a falsy value.

## Solution

The solution replaces the loose equality (`==`) with strict equality (`===`). Strict equality only returns `true` if both values are of the same type and have the same value, making the null check more reliable and preventing unexpected results.

## How to run

1. Clone this repository.
2. Open `bug.js` and `bugSolution.js` in your preferred JavaScript environment or IDE.
3. Execute the code using Node.js (or another JavaScript runtime) and observe the output to compare the behavior of both versions.