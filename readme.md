This library can solve any puzzle that can be written as a transition function on a byte array.
This assumes that there is a small (in the millions) set of possible states to transition to.

It works probabilistically, and occasionally will falsely treat a new state as already visited.
This means the solver will have some false negatives where it thinks a puzzle is unsolvable that is solvable.
It does not have false positives (unless there is a bug).

See `test/solver-tests.keen` for an example.
