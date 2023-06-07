# Debugging 

 
## What is Debugging?
\
Debugging is the process of finding and fixing errors or bugs in the source code of any software. When software does not work as expected, computer programmers study the code to determine why any errors occurred.


The main **objective** of Debugging is to find the exact root cause at code level to fix the errors and bugs found during the testing.

\
**Flowchart of basic Debugging:**

![debugging flowchart](./images/debuggingFlowchart.png)

Always debug the program for the simplest input that produces the bug. Solving a bug in the simplest case brings you closer to solving it in the general case; to solve a problem, solve a simpler sub-problem.

A bug fix should always be accompanied by a unit test. This guarantees that future bugs won't be caused by this bug and that you won't have to waste time fixing the same bug again.

To file a bug, give a list of steps that reliably cause the bug, and state the difference in expected and actual outcomes. Use the simplest input possible by starting with an input that causes the problem and simplifying it until it can't be simplified without the problem going away.

### Production debugging

Production debugging is the process of finding bugs and errors within an application during its production environment and determining the cause of the error.

Production debugging poses various challenges, such as having to troubleshoot the app and disturbing its performance. Moreover, making changes to the program while it is running might lead to unanticipated outcomes for users and interfere with their overall user experience.