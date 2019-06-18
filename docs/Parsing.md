# Parser documentation

Like every other compilers, Chirp has a parser. This *obviously* is the documentation for that parser. You might want to check out the parse tree documentation too.

## Example

> This exemple is with the rewritten parser, but it isn't written yet. lmao

In this simple example we will see how the parser should behave during parsing.

```chirp
int: a = 123
```

First the string will be separated in words, inside a vector. All spaces will be removed. Then an unranged list of tokens will be made, 
those tokens have a type and value such as those in the board bellow:

| Token | Lexeme |
| --- | --- |
| **OBJECT_TYPE_TOKEN** | int |
| **TREE_UNDEFINED_TOKEN** | : |
| **OBJECT_IDENTIFIER_TOKEN** | a |
| **VAR_CONFIRM_TOKEN** | = | 
| **VALUE_INTERGER_TOKEN** | 123|

These token actually works, but are subjec to change.

Then after this unorganized cluster of Tokens has been generated, the parser will go trought it an create a parse tree. The parse tree
will be very usefull, as it will be used to do stuff such as writing the assembly code. The parse tree contains all the tokens in a 
hierachical and organized manner.

# Detailed process

This section will be worked on later, be free to write it yourself!
