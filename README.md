Mathmulator
===========

The Mathmulator is a simple arithmetic problem solver with a
command-line interface.  At the moment, it supports only very basic
two-input calculations:

* addition: 2 + 5 = 7
* subtraction: 5 - 2 = 3
* multiplication: 5 * 2 = 10
* division: 5 / 2 = 2.5
* modulo: 5 % 2 = 1
* power: 5 ^ 2 = 25

Interaction with the Mathmulator begins by invoking the tool.  Do this
by running `program`.

```
$ ./program
Enter an expression (use spaces): 
```

(Note that on Windows, this process may be a bit more involved.)

The Mathmulator also supports a very simple answer register feature.
The character `#` may be used to refer to the most recent successful
answer in the calculation:

```
Enter an expression (use spaces): 3 + 5
8
Enter an expression (use spaces): # ^ 2
64
Enter an expression (use spaces): 
```

Be careful to obey the prescribed input format precisely.  You must
include whitespace around the operator, or the parser will choke:

```
Enter an expression (use spaces): 3 +   5
8
Enter an expression (use spaces):   3    +   5    
8
Enter an expression (use spaces): 3 +5
Bogus expression (wrong number of pieces).
Enter an expression (use spaces): 
```
