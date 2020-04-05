
## Scala helpful compiler errors

A list of Scala compiler errors that could be more helpful, especially for newcomers to Scala.

The list is focused on Scala 3's Dotty compiler. One day this list could be useful for a [larger project](https://contributors.scala-lang.org/t/towards-better-error-messages-in-scalac/1470/31) around compiler errors. Such a project seems unlikely to occur for Scala 2.13's scalac, which is why this list is Dotty-specific.

## Pull requests welcome

🛠️ Help by submitting pull requests with Dotty errors that could be more helpful, especially for newcomers to Scala.

Use this template:

#### $errorName

* [Scastie example](https://scastie.scala-lang.org/G4zbEq5dTFqSnRryRnTzwg)
* Current error msg:
```
// paste output of dotty compiler error or warning
```
* Example helpful msg: `Oh no, it broke. Suggestion: don't break it`

## List of Dotty compiler errors that could be more helpful

### If statement missing an else branch

* [Scastie example](https://scastie.scala-lang.org/G4zbEq5dTFqSnRryRnTzwg)
* Current error msg:
```
Found:    Unit
Required: Int
```
* Example helpful msg: `The result type of this if statement must be an Int, but there's no else branch, so it returns Unit on else. Suggestion: add an else branch`
