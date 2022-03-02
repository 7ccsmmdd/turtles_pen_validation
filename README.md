## A simple validator checking the pen state of a turtle programs

Write a validator that issues a warning if it is possible that at the end of a turtle program the pen may not be down (this may indicate a program that hasn't drawn anything).

For example, 

```
turn right by 1 degrees
forward(10)
forward(10)
turn left by 360 degrees

pen up
```

should add a yellow wriggly line under the statements (will typically be shown under the first statement) with the warning message `This program may not end with the pen down`.

As always, you may have to generate xtext artifacts after your initial download of the code.

Eventually, you should get 10/10 from the auto-grader. When running the corresponding tests from Eclipse, you may find the Xpect feedback particularly helpful. In particular, when a test fails, you can double click on the first line of the stack trace to see a diff of the TurtleProgram text and warnings that the test was expecting and what was actually seen. This can make tracking down the source of a problem much easier.
