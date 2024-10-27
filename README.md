# Lols scripting language

## Building


## Grammar Definition
Grammar in variant of Backus-Naur form
```
expression : equality
equality   : comparison (( "==" | "!=") comparision)*;
comparison : term (("<" | "=<" | ">" | "=>") term)*;
term       : factor (("+" | "-") factor)*;
factor     : unary ( ("/" | "*") unary)*;
unary      : ("!" | "-") unary | primary;
primary    : NUMBER | STRING | "true" | "false" | "nil | "(" expression ")";
```

## Learning Goals
As stated in the introduction, the aim of this interpreter is for me to learn about language hacking.
Here are my learning goals:
- [x] Learn how to make a Scanner
- [x] Learn about the Visitor design pattern
- [ ] Learn about the Backus-Naur Form
- [ ] Re-learn about Recursive Descent Parsers