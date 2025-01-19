# Stack Overflow in Recursive Factorial Function

This repository demonstrates a common error in recursive functions: stack overflow. The `bug.hack` file contains a recursive factorial function that will fail for large inputs due to exceeding the call stack limit.  The `bugSolution.hack` file provides a corrected iterative solution.

The issue arises because each recursive call adds a new frame to the call stack.  For large inputs, this can exhaust the available stack space, leading to a stack overflow error. The iterative solution avoids this by using a loop and accumulating the result without recursive calls.