# PHP Loose Comparison Pitfall: '0' == false

This repository demonstrates a common, yet subtle, error in PHP related to loose comparison (`==`) when dealing with strings and booleans.  Specifically, the string '0' is loosely equal to the boolean `false` in PHP.

The `bug.php` file shows the problem. The `bugSolution.php` file illustrates the correct approach using strict comparison (`===`).

This unexpected behavior can lead to hard-to-debug issues in PHP applications. Always use strict comparison (`===`) unless you explicitly intend to rely on loose comparison's type juggling behavior.  Strict comparison ensures that both the value and the type of the operands are identical, making your code more robust and predictable.