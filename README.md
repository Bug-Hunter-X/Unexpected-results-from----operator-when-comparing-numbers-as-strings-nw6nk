# Tcl Bug: Unexpected == behavior with numbers represented as strings

This repository demonstrates a common error in Tcl where the `==` operator's string-based comparison leads to incorrect results when comparing numbers stored as strings.

## The Bug

The `bug.tcl` file contains a procedure `badproc` that intends to compare two numbers. However, because it uses `==` for comparison, it compares them lexicographically (as strings), leading to incorrect outcomes.

## The Solution

The `bugSolution.tcl` file shows how to correctly compare numbers in Tcl using the `expr` command for numerical comparison.

## How to Reproduce

1.  Clone this repository.
2.  Run `tclsh bug.tcl`. Observe the unexpected results.
3.  Run `tclsh bugSolution.tcl`. Observe the correct results.