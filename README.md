# Smile: An SML Preprocessor

Grammar not yet finalized

## Grammar

(forked from SML Grammar: http://www.mpi-sws.org/~rossberg/sml.html)
See grammar.tex and grammar.pdf

## Specific Changes from SML

* `{ }` for scope instead of `let ... in ... end`

* `-` instead of `~` for negative numbers

* `+` instead of `^` for string concatenation

* `&&` instead of `andalso`, `||` instead of `orelse`

* `if <exp> { <exp> } else { <exp> }` instead of `if <exp> then <exp> else <exp>`

* `while <exp> { <exp> }` instead of `while <exp> do <exp>`

* Scala-style `<exp> match { <match>* }` instead of `case <exp> match { <pattern>* }`

* Scala-style patterns `case <pattern> => <match>` instead of `<pattern> => <match>`

* Characters are single-quoted instead of the `#`-syntax

* Remove `fn` for anonymous functions (ie just like `() => 3` instead of `fn () => 3`

* Record selection is `record#label` (binds tightly) instead of `#label record`

