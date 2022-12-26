# mp-spdz-cheatsheet
Tips and Tricks for using MP-SPDZ

## Cheatsheet

- Prefer runtime loops over compile time loops
- Use pypy with ./compile.py to make compilation faster
- Use `MemValue` to pass parameters across runtime loops
- For simulating a matrix using an `OptimalOram`, map entry `i,j` to `i * n_columns + j`
- Prefer iterative algorithms over recursive algorithms
