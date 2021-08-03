# pykoop

Koopman operator identification library in Python.

## To do

### General

- [x] Examples and doctests
- [ ] Fix idempotence unit test if possible?

### Pipeline

- [ ] Add post-processing step for normalization of quaternions etc.
- [x] Fix examples (Must merge LMI methods first)
- [ ] Handle methods that don't save a `coef_`?
- [ ] Cosmetic: Replace ints with floats in function signature?
- [x] Merge LMI methods with new abstract base class

### LMI

- [ ] Add nonhomog test case
- [ ] Adjust fit and predict testing to avoid skipped tests. Parametrize
  arguments for fixtures?
- [x] Rename `_base_problem` to `_get_base_problem`
- [x] Rename `U_` to `coef_`
- [x] Remove constraint-adding functions and wrap them inside an inherited
  `_base_problem`? Might cause problems when trying to mix regularizers.
- [x] Make `_add_regularizer` return a problem instead of acting in-place?
