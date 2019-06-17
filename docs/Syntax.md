## Syntax

Chirp's syntax is a weird mix between C's and Python's syntax, giving a low-level but modern programming language.

An example written in Chirp code:
```chirp
  import <io>

  int Add (x, y)
  {
    return x + y
  }

  entry int start ()
  {
    int: result = Add (1, 2)
    print (result)
  }
```

<br>

### Keywords

Chirp has a specific set of words, *keywords*, that's reserved in the Chirp language. These keywords has a very specific meaning in the context of the source code. Keywords:
```chirp
  if elif else entry inner int float char string true false null import
  for while state switch case return class
```

<br>

### Comments

In Chirp we support both single line comments:
```chirp
  # I'm a single line comment
```
And multiline comments:
```chirp
  ###
    I'm
    a
    multiline
    comment!
    :)
 ###
```

<br>

### Import

> Imports in Chirp are **always** relative!

Importing in Chirp is very simple. Here's a simple example:
```chirp
  import <io>
```
This imports the io library. These are all of the built-in libraries:
As of june 17 2019, none of theses libraries have been written yet, but they are coming!
- io
- eve
- json
- math

To import a file, let's say you wanna import your helper file: `SuperHelper.ch`. But that file is in your `Helpers` folder. Then you just do:
```chirp
  import <Helpers.SuperHelper>
```
You replace `/` in your path with `.`, and you just remove the file ending. Chirp will do that itself.

> To read more about the imports of Chirp, head to `Imports.md`
