# ORDER OF EXECUTION:
The JavaScript interpreter uses the concept of execution contexts. There is one global execution context; plus, each function creates a new new execution context. They correspond to variable scope.


Each time a script enters a new execution context, there are two phases
of activity:
 ### PREPARE
-  The new scope is created
- Variables, functions, and arguments are created
-  The value of the this keyword is determined

 ###  EXECUTE
- Now it can assign values to variables
- Reference functions and run their code
-  Execute statements

**The JavaScript console will tell you when there is a problem with a script,
where to look for the problem, and what kind of issue it seems to be.**

#### BREAKPOINTS:

You can pause the execution of a script on any
line using breakpoints. Then you can check the
va lues stored in variables at that point in time.

- JavaScript has 7 different types of errors. Each creates
its own error object, which can tell you its line number
and gives a description of the error.
