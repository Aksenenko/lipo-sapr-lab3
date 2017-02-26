teach-lex-polska-calc
=====================

Demo project for LEX.

Calucates expressions in reverse (polska) notations 

Supported:
* integers
* 4 math operations (+, -, *, /)
* multiplicities operations (intersection, union and checking number in multiplicity). 
Syntax of multiplicity operations:
* intersection: [..] [..] *m
* union: [..] [..] +m
* checking number in multiplicity: [..] number ?

For using this calculator just 
```makefile
make
``` 
him and use the standart input for parsing math operations.

Example 1: 2+2*2
```c
2 2 2 * +
```

Example 2: [1,2,3] intersection with [1,2]
```c
[1,2,3] [1,2] *m
```

Example 3: (([1,2,3] intersection with [3]) union with [4,5]) is 1 in multiplicity
```c
[1,2,3] [3] *m [4,5] +m 1 ?
```
