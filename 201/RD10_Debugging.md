# Read 10 Debugging

## Chapter 10 Java Script

- **execution context** Every statement in a script lives in one of these three below
  - **Global Context** Code that is in the script, but not in a function. There is only one global context in any page.
  - **Function Context** Code that is being run within a function. Each function has its own function context
  - **Eval Context** Text is executed like cade in an internal function called eval() 
- **Variable Scope** The first two execution contexts correspond with the notion of scope 
  -**Global Scope** If a variable is declared outside a function, it can be used anywhere because it has global scope. If you do not use the var keyword when creating a variable, it is placed in global scope
  - **Function-level scope** When a variable is declared within a function it can only be used within that function
- **The Stack** JS interpreter processes one line of code at a time. When a statement needs data from another function, it stacks the new function on top of the current task.
- **Execution of context & Hoisting** Each time a script enters a new execution contex there are two phases of activity
  - Prepare
    - The new scope is created
    - variables, functions and arguments are created
  - Execute
    - Now it can assign values to variables
    - reference functions and run their code
    - execute statments
- **Error Objects** can help you find where your mistakes are and browsers have tools to help you read them
  - **SyntaxError** This is caused by incorrect use of the rules of the language. (typo)
  - **ReferenceError** This is caused by a variable that is not declared or is out of scope
  - **TypeErroe** Caused by trying to use an object or method that does not exist
  - **Range Error** If you call a function using numbers outside of its accepted range.
- **Logging Data To the Console**
  1. The first line is used to indicate the script is running
  2. event handler waits for the user leaving a text input and logs the value that they entered into the form field
  3. That the user clicked submit
  4. The value in the width input
  5. The value in the height input
  6. The value of the area variable

### Console Methods

1. `console.info()` can be used for general information
2. `console.worn()` can be used for warnings
3. `console.error()` can be used to hold errors.

### Grouping Messages

1. `console.group()` If you want to write a set of related data to the console to group the messages together
2. `console.groupEnd()` indicates the end of the group

- `console.table()` lets you output a table showing objects and arrays that contain other objects or arrays.
- `console.assert()` you can test if a condition is met, and whrite to the console only if the expression evaluates to false
- **Breakpoints** You can pause the execution of a script on any line using breakpoints. Then you can check the values stored in variables at that point in time.
- **Conditional Breakpoints** You can indicate that a breakpoint should be triggered only if a condition that you specify is me. The condition can use existing variables
- **Debugger Keyword** Can be used to create a breakpoint in your code using just the debugger keyword

### Handling Exceptions

- *Try* First specify the code that you think might throw and exception within the try block
- *catch* If exception catch steps in with an alternative set of code
- *Finally* The contents of the finally code block will run either way wheather the try block succeeded or failed.
- **Throwing Errors** To create you own error, you use `throw new Error('message');`
