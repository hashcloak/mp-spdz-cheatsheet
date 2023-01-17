# mp-spdz-cheatsheet
Tips and Tricks for using MP-SPDZ

## Cheatsheet

- Prefer runtime loops over compile time loops
- Use pypy with ./compile.py to make compilation faster
- Use `MemValue` to pass parameters across runtime loops
- For simulating a matrix using an `OptimalOram`, map entry `i,j` to `i * n_columns + j`
- Prefer iterative algorithms over recursive algorithms
- When needing to do while loops in which the condition uses a secret-shared number, use `@while_do` instead of a Python `while` loop
- If you want to pass in extra variables that were defined outside of a `@for_range` of `@while_do` and they need to be modified, use `.iadd` (or equivalent) or add `nonlocal` to the variables declaration
- Using `-l` when compiling with `compile.py` will convert all your Python loops to runtime loops
