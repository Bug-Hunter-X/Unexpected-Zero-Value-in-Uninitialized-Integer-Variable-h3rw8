# Go: Unexpected Zero Value in Uninitialized Integer Variable

This repository demonstrates a common yet subtle issue in Go: unexpected behavior when using uninitialized variables.  Specifically, it highlights the default zero value of integer variables and how to handle it.

## The Problem

Go initializes variables to their zero values if not explicitly assigned a value. For integers, the zero value is 0. This behavior can be unexpected if not considered, especially in larger programs or concurrent scenarios.

## The Solution

The provided `bugSolution.go` file addresses this issue by explicitly initializing the integer variable `i` before use, thus avoiding the default zero value problem.

Always initialize your variables to ensure predictable and correct program behavior. Using explicit initialization is more readable and helps prevent runtime surprises.