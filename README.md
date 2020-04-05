
## What is scala-helpful-compiler-errors?

scala-helpful-compiler-errors is a list of Scala compiler errors that could be more helpful, especially for newcomers to Scala.

Experienced Scala programmers maintain a mental map of compiler error -> actual problem. In many cases a compiler error can't know the "actual" problem, but in many cases it can or make a helpful guess.

The list of compiler errors focused on Scala 3's Dotty compiler. The idea behind this project is to build up a list of compiler errors that could one day be an input into a [larger project](https://contributors.scala-lang.org/t/towards-better-error-messages-in-scalac/1470/31) to make compiler errors more helpful. Such a project seems unlikely to occur for Scala 2.13's scalac, which is why this list is Dotty-specific.

## PRs Welcome

Please submit pull requests with Dotty errors that could be more helpful, especially for newcomers to Scala.

## Template for new compiler errors or warnings

#### $errorName

* Scastie link: $scastieLink (here's a [starter](https://scastie.scala-lang.org/G4zbEq5dTFqSnRryRnTzwg))
* Current error msg:
```
// paste output of dotty compiler error or warning
```
* Suggested helpful msg: `Oh no, it broke. Suggestion: don't break it`

## List of Dotty compiler errors that could be more helpful

#### If statement missing an else branch

* Scastie link: https://scastie.scala-lang.org/G4zbEq5dTFqSnRryRnTzwg
* Current error msg:
```
Found:    Unit
Required: Int
```
* Suggested helpful msg: `The result type of this if statement must be an Int, but there's no else branch, so it returns Unit on else. Suggestion: add an else branch`
