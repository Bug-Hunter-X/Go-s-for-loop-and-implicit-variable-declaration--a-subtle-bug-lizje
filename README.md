# Go's for loop and implicit variable declaration: a subtle bug
This repository demonstrates a common subtle bug in Go involving `for` loops and implicitly declared variables within the loop's initializer.

The bug is caused by the implicit declaration of the loop variable within the `for` loop's initialization. This can lead to unexpected behavior if you're not careful.

## The Bug
The `bug.go` file contains the buggy code. It demonstrates a simple `for` loop that iterates while `i` is less than 10. The issue is that `i` is declared implicitly within the for loop, and this can lead to issues if the condition is not properly handled.

## The Solution
The `bugSolution.go` file provides a corrected version of the code. It explicitly declares the loop variable outside the loop's initialization, avoiding the potential ambiguity and unexpected behavior.