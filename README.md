Simple precedence parser&evaluator for arithmetic expressions with +, *, - and parenthesization.

The specific grammar supported is:
``` 
S ::= E eof
E ::= T ((+|-) T)* 
T ::= F (* F)*   
F ::= -F | G
G ::= num | lparen E rparen
```

Build on top of simpleAST@[COMP520](https://www.cs.unc.edu/~prins/Classes/520/)