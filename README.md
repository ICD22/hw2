# ICD22 Homework2

## How port your homework1 to homework2

1. remove the main from the scanner.l
2. remove all the `#define [TOKEN] [INDEX]` in `scanner.l` (we define them in parser.y with `%token`)
3. add `#include "parser.h"` in your `scanner.l`
4. add a `#pragma token on` and `#pragma token off` to control `[INFO]` and `token(type:...)...` message, default is off

Please follow the grammar in `01-minipascal-spec.pdf ` to write your syntax rule in `parser.y`.

## Some useful online information
[lex & yacc](http://dinosaur.compilertools.net/#lex)
