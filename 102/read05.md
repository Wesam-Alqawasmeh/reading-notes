# Javascript operators 

- JavaScript operators are used to assign values, compare values, perform arithmetic operations, and more.

### Arithmetic operators 

Arithmetic operators are used to perform arithmetic between variables and/or values.

| Operator	      | Description |
| ----------- | ----------- |
|+      | Addition      |
| -   | Subtraction       |
| * | Multiplication|
| / | Division |
| % | Modulus (division remainder) |
| ++ | Increment |
| -- | Decrement |


### Assignment operators

Assignment operators are used to assign values to JavaScript variables.

| Operator      | Example | Same as     |
| ----------- | ----------- | ----------- | 
| =     | 	x = y      | x = y |
| +=  | x += y      | x = x + y |
|-= |  x -= y | x = x - y |
| *= | x *= y | x = x * y |
| /= | x /= y | 	x = x / y |
| %= | x %= y | x = x % y | 


### Comparsion operators

Comparison operators are used in logical statements to determine equality or difference between variables or values.

| Operator      | Description |
| ----------- | ----------- |
| ==      | equal to      |
| ===   | equal value and equal type       |
| != | not equal | 
| !== | not equal value or not equal type| 
| > | greater than | 
| < | less than | 
| >= | 	greater than or equal to| 
| <= | less than or equal to|


### Logical operators

Logical operators are used to determine the logic between variables or values.

|Operator     | Description |
| ----------- | ----------- |
| &&      | and      |
| ||  | or       |
| ! | not |


## JS loops (for & while) :

**for**

A for loop repeats until a specified condition evaluates to false.

*for ([initialExpression]; [conditionExpression]; [incrementExpression])
  statement*

When a for loop executes, the following occurs:

1. The initializing expression initialExpression, if any, is executed. This expression usually initializes one or more loop counters, but the syntax allows an expression of any degree of complexity. This expression can also declare variables.
2. The conditionExpression expression is evaluated. If the value of conditionExpression is true, the loop statements execute. If the value of condition is false, the for loop terminates. (If the condition expression is omitted entirely, the condition is assumed to be true.)
3. The statement executes. To execute multiple statements, use a block statement ({ ... }) to group those statements.
4. If present, the update expression incrementExpression is executed.
5. Control returns to Step 2


**while**

A while statement executes its statements as long as a specified condition evaluates to true. A while statement looks as follows:

*while (condition)
  statement*

  If the condition becomes false, statement within the loop stops executing and control passes to the statement following the loop.

The condition test occurs before statement in the loop is executed. If the condition returns true, statement is executed and the condition is tested again. If the condition returns false, execution stops, and control is passed to the statement following while.

To execute multiple statements, use a block statement ({ ... }) to group those statements
