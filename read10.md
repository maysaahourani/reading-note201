## chapter 10 (error handling&debugging) :
1. EXECUTION CONTEXT :
2. GLOBAL CONTEXT
3. FUNCTION CONTEXT .
EVAL CONTEXT (NOT SHOWN)
**EXECUTION** CONTEXTS: The JavaScript interpreter uses the concept of execution contexts. There is one global execution context; plus, each function creates a new new execution context. They correspond to variable scope.

* EXECUTION CONTEXT & HOISTING:
PREPARE: The new scope is created Variables, functions, and arguments are created The value of the this keyword is determined EXECUTE: Now it can assign values to variables. Reference functions and run their code . Execute statements.

* VARIABLE SCOPE :
GLOBAL SCOPE .
FUNCTION-LEVEL SCOPE .
Each time a script enters a new execution context, there are two phases of activity:
PREPARE .
EXECUTE .
error

***HOW TO DEAL WITH ERRORS***: Now that you know what an error is and how the browser treats them, there are two things you can do with the errors.
DEBUG THE SCRIPT TO FIX ERRORS If you come across an error while writing a script (or when someone reports a bug), you will need to debug the code, track down the source of the error, and fix it.

* HANDLE ERRORS GRACEFULLY: You can handle errors gracefully using try, catch, throw, and f i na1ly statements. Sometimes, an error may occur in the script for a reason beyond your control. For example, you might request data from a third party, and their server may not respond. In such cases, it is particularly important to write error-handling code.

* DEBUGGER KEYWORD: You can create a breakpoint in your code using just the debugger keyword. When the developer tools are open, this will automatically create a breakpoint.
You can also place the debugger keyword within a conditional statement so that it only triggers the breakpoint if the condition is met. This is demonstrated in the code below.

***it is particularly important to remember to remove these statements before your code goes live as this could stop the page running if a user has developer tools open.***