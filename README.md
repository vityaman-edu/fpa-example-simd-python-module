# FPA Optional Task

## Descriptions

Was implemented 2 function written in `C` programming
language to count non-negative
numbers.
The first is just trivial for-loop and the second uses SIMD.
They was packed in native `Python` module and tested using `unittest` from Python stdlib. Was done on the second semester of ITMO CSE Bachelor.

- [Report](./pymodule/pysimd/README.md)

## SIMD diving in

### Links

- Intel intrinsics guide: https://www.intel.com/content/www/us/en/docs/intrinsics-guide/index.html

- VTune Profiler:
https://www.intel.com/content/www/us/en/developer/tools/oneapi/vtune-profiler.html

## How to create an external c module for python

### Links Guide

- https://docs.python.org/3/extending/extending.html
- https://docs.python.org/3/library/array.html

### Compile c implementation

```bash
gcc -Wall -I /usr/include/python3.8/ a.c -o a
```

### Add module to interpreter

```bash
python3 setup.py install
```
