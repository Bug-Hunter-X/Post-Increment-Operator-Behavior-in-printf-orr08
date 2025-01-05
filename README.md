# Post-Increment Operator Behavior in printf
This repository demonstrates a common yet subtle error in C programming involving the post-increment operator in combination with the printf function.

## The Bug
The provided C code snippet exhibits unexpected behavior due to the post-increment operator (x++) used within the printf function with multiple arguments. The post-increment operator increments the variable *after* its current value is used.

## The Solution
The solution focuses on understanding the order of evaluation within the printf statement. To achieve the intended result, either separate print statements or intermediate variables can be used to ensure predictable behavior.

## How to run the code
1. Save the bug.c and bugSolution.c code snippets.
2. Compile the code using a C compiler (like GCC):  gcc bug.c -o bug && gcc bugSolution.c -o bugSolution
3. Run the executables: ./bug and ./bugSolution