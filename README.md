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

### Using the repository

There are two ways to do this activity:

1. You can check out the repository and import the projects into Eclipse, then do the activity there. Commit your changes and push them back to GitHub to trigger the autograding so you can see whether you've correctly implemented the validator. More information about checking out and editing code in Eclipse can be found on KEATS.
2. You can do this activity in your browser.

   Due to an annoying, long-standing GitHub Classroom bug, you need a small extra step for this:

    1. Copy the URL of your repository (see the location bar of your browser).
    2. Open [this form](https://7ccsmmdd.github.io/) and paste your repository URL into the corresponding field.
    3. The URL field should fill with a long complicated URL as soon as you move out of the text field. 
    4. Click on the button at the bottom of the form to open that URL in a new tab: this is the MDENet Education Platform with the activity pre-loaded. Edit the validator code, generate the Xtext editor, then you can open a playground view where you can experiment with the validations. **Note that you must save your changes before switching to the generated editor or you will lose them.** Saving your changes will create a commit in your repository, which will also automatically trigger the autograding process.