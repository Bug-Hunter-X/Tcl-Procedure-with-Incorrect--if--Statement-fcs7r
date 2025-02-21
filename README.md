# Tcl Procedure with Incorrect 'if' Statement

This repository demonstrates a common error in Tcl procedures involving the incorrect use of the `if` statement and `return` command. The `badproc` procedure is designed to return the larger of two inputs. However, due to the placement of the `return` statements, it only returns the result of the first condition check, resulting in incorrect output.

The `bugSolution.tcl` file presents a corrected version of the procedure that addresses the error.

## How to reproduce the bug

1. Run `bug.tcl`
2. Observe the unexpected output (only returns the first value if its larger)

## How to fix the bug

Review `bugSolution.tcl` to see the corrected implementation. The solution uses a `return` statement after the `if` statement to ensure both cases are handled correctly.