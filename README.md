## A name validator for turtle programs

Write a simple validator for your turtle program language, that issues a warning for every variable declaration where the variable name starts with an upper case character.

For example, 

```
var VarWithWrongName = 7
```

should add a yellow wriggly line under the word `VarWithWrongName` with the warning message `Variable name should start with a lowercase character`.

As always, you may have to generate xtext artifacts after your initial download of the code.

Eventually, you should get 10/10 from the auto-grader. When running the corresponding tests from Eclipse, you may find the Xpect feedback particularly helpful. In particular, when a test fails, you can double click on the first line of the stack trace to see a diff of the TurtleProgram text and warnings that the test was expecting and what was actually seen. This can make tracking down the source of a problem much easier.
