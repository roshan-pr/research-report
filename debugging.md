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

### Steps involved in debugging are:

**Step 1: Identify the Error**

This is the first stage of Debugging is identifying the actual Error in the code of the software.

**Step 2: Find the error Location**

Once the problem has been identified, you will need to thoroughly review the code several times to identify the precise location of the error. This stage, in general, focuses on locating the error rather than perceiving it.

**Step 3: Analyze the error**

The third step is error analysis, which is a bottom-up technique that starts with identifying the issue and then analyses the code. This stage helps in the understanding of the errors. error analysis has two major goals: reevaluating errors to identify existing bugs and proposing the uncertainty of incoming collateral damage in a fix.

**Step 4: Prove the analysis**

After examining the primary bugs, it is necessary to search for any additional issues that may show on the program. The fourth step is used to develop automated tests for such domains by integrating the test framework.

**Step 5: Cover Lateral Damage**

The fifth phase involves collecting all of the unit tests for the code that has to be modified. When you run these unit tests, they must pass.

**Step 6: Fix & Validate**

The final stage is fix and validation, which focuses on resolving defects before running all of the test scripts to determine if they pass.


### There are several common methods and techniques used in debugging, including:

- **Code Inspection:** This involves manually reviewing the source code of a software system to identify potential bugs or errors.

- **Debugging Tools:** There are various tools available for debugging such as debuggers, trace tools, and profilers that can be used to identify and resolve bugs.

- **Unit Testing:** This involves testing individual units or components of a software system to identify bugs or errors.

- **Integration Testing:** This involves testing the interactions between different components of a software system to identify bugs or errors.

- **System Testing:** This involves testing the entire software system to identify bugs or errors.

- **Monitoring:** This involves monitoring a software system for unusual behavior or performance issues that can indicate the presence of bugs or errors.

- **Logging:** This involves recording events and messages related to the software system, which can be used to identify bugs or errors.

### Production debugging

Production debugging is the process of finding bugs and errors within an application during its production environment and determining the cause of the error.

Production debugging poses various challenges, such as having to troubleshoot the app and disturbing its performance. Moreover, making changes to the program while it is running might lead to unanticipated outcomes for users and interfere with their overall user experience.
