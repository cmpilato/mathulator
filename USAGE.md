Mathmulator Usage
=================

General usage of the Mathmulator involves entering simple mathematical
expressions at the prompt:

```
Enter an expression (or 'help'): 3 + 5
8
Enter an expression (or 'help'): 5 ^ 2
25
Enter an expression (or 'help'): 
```

The Mathmulator also supports a very simple answer register feature.
The character `#` may be used to refer to the most recent successful
answer in the calculation:

```
Enter an expression (or 'help'): 3 + 5
8
Enter an expression (or 'help'): # ^ 2
64
Enter an expression (or 'help'): 
```

Be careful to obey the prescribed input format precisely.  You must
include whitespace around the operator, or the parser will choke:

```
Enter an expression (or 'help'): 3 +   5
8
Enter an expression (or 'help'):   3    +   5    
8
Enter an expression (or 'help'): 3 +5
Bogus expression (wrong number of pieces).
Enter an expression (or 'help'): 
```

One exception to the operand-operator-operand required input is the
support for calculator-style memory actions:

* M+:  Add the value of the most recent successful calculation to the value stored in memory.
* M-:  Subtract the value of the most recent successful calculation from the value stored in memory.
* MC:  Clear the memory register (reset to 0).
* MR:  Recall the memory register -- that is, print its value.

Other miscellaneous commands which are supported include:

* q:  Quit the program.