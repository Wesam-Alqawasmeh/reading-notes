# Debugging


## ORDER OF EXECUTION

- To find the source of an error, it helps to know how scripts are processed.
The order in which statements are executed can be complex; some tasks
cannot complete until another statement or function has been run.

## EXECUTION CONTEXTS

- The JavaScript interpreter uses the concept of execution contexts. There is only one global execution context; in addition, each function creates a new new execution context. They correspond to variable scope.


**Excution context**

1. GLOBAL CONTEXT.
2. FUNCTION CONTEXT.
3. EVAL CONTEXT. 

**Variable scope**

1. GLOBAL SCOPE.
2. FUNCTION-LEVEL SCOPE.

![order](https://miro.medium.com/max/2000/1*ACtBy8CIepVTOSYcVwZ34Q.png)




## EXECUTION CONTEXT & HOISTING

**Acticities**


1. PREPARE.
2. EXECUTE. 

![EXECUTE](https://whynotgoogleit.com/wp-content/uploads/2020/05/JavaScript-Global-Execution-context-execution-phase.jpg)


## UNDERSTANDING SCOPE

- In the interpreter, each execution context has its own variables object. It holds the variables, functions, and parameters available within it. Each execution context can also access its parent's variables object.

- If a variable is not found in the variables object
for the current execution context, it can look in the
variables object of the parent execution context.
But it is worth knowing that looking further up the
stack can affect performance, so ideally you create
variables inside the functions that use them.


## ERROR OBJECTS

**properties of error object**

PROPERTY | DESCRIPTION
--------- | ------------ 
name | Type of execution
message | Description
fileNumber | Name of the JavaScript file
lineNumber | Line number of error


**built-in error objects**

OBJECT | DESCRIPTION 
------- | -----------
Error | Generic error - the other errors are all based upon this error
SyntaxError | Syntax has not been followed
ReferenceError | Tried to reference a variable that is
not declared/within scope
TypeError | An unexpected data type that
cannot be coerced
RangeError | Numbers not in acceptable range
URIError | encodeURI ().decodeURI(),and
similar methods used incorrectly
EvalError | eva l () function used incorrectly

**HOW TO DEAL WITH ERRORS**

1. DEBUG THE SCRIPT TO FIX ERRORS.
2. HANDLE ERRORS GRACEFULLY. 

## A DEBUGGING WORKFLOW

- WHERE IS THE PROBLEM?

1. Look at the error message.
2. Check how far the script is running.
3. Use breakpoints where things are going wrong.

- WHAT EXACTLY IS THE PROBLEM?

1. When you have set breakpoints, you can see if the
variables around them have the values you would
expect them to.
2. Break down / break out parts of the code to test
smaller pieces of the functionality.
3. Check the number of parameters for a function, or
the number of items in an array.


**BREAKPOINTS**

- You can pause the execution of a script on any
line using breakpoints. Then you can check the
va lues stored in variables at that point in time.


![debugging](https://cdn.educba.com/academy/wp-content/uploads/2019/09/What-is-Debugging.png)

