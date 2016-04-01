Mathmulator Usage
=================

General usage of the Mathmulator involves entering simple mathematical
expressions at the prompt:

```
Enter an expression (use spaces): 3 + 5
8
Enter an expression (use spaces): 5 ^ 2
25
Enter an expression (use spaces): 
```

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
