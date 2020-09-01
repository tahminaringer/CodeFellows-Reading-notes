# JavaScript

- script is a series of instructions
- Scripts allow browser to check situation and perform appropriate steps
- Scripts are instructions computer follows step by step

## Writing Script

- first state goal
- then list tasks
- program must give computer enough detail to perform task everytime like it was first time

### Define goal

- define the task you want to complete

### Design the Script

- split goal into two series of tasks. Use flow chart.
- separate out all tasks using flow chart
- break down into sequence of steps.

### Code Each Step

- write each step in progaming language.
- Always design script first

### Steps to code

- Every step from flowchart needs to be written in code
- detail every step
- *debugging* solve issues
- learn to think like computer
- *progamatically* computers follow series of steps
- computer looks at each step individually once it completes this it can give an answer

## Defining a goal

1. detail your goals/what do you want to achieve
2. Breakdown into a series of steps

    - script is triggered when button is pushed
    - it collects name entered
    - checks that user entered a value
    - if nothing enter, message will appear promting them to enter name
    - If name entered, will perform next task
    - show ending result

## Sketching Flowchart

- flowcharts show path between steps
- arrows show how script moves through tasks

## Expressions

- expressions that just assing a value to a variable `var color = 'beige'`
-expressions that use 2 or more values to get single value. `var area = 3 * 2`

## Operators

- Allow programers to creat a single value form 1 or more values
- *Assignment Operators* `color = 'beige';` asigns value to variable
- *Arithmetic Operators* `area = 3 * 2;` performs basic math
- *String* `greeting = 'Hi' + 'Molly';` Combines to values to read Hi Molly.
- *Comparison Operators* `buy = 5 > 3;`
- *Logical Operators* `buy = (5 > 3) && (2 < 4);` Combine expressions and returns true or false

## Arithmetic Operators

- `+` addition
- `-` subtraction
- `/` divides two values
- `*` Multiplies
- `++` increment- adds 1 to the current number `i = 10; i++; 11`
- `--` decrement- subtracts 1 from the current number `i=10; i--; 9`
- `%` modulus - divides two values and returns the remainder `10%3; 1`

## String Oporator

- String oporator is `+`
- string oproator joins 2 or more strings to create a single value also called **concatenation**

## Function

- functions let you group a series of statements to gether to perform a specific task
- if different parts of a scrpt repeat the same task you can reuse the function instead of repeating the same statment
- helps organize code
- stores steps needed to achieve a task
- calling the fuction is asking it to perform its task
- **parameters** pieces of information passed to a function
- **return value** the expected answer to a function
- **Declaring the function**
  - `function sayHello() {`
      `document.write('hello');`
- **Calling a Function**
  - `sayHello();`
- **Declaring Functions that need Information**
  - `function getArea(width, height) {`
      `return width * height;`
- **Calling functions that need information**
  - **Arguments as Values**`getArea(3, 5);`
  - **Arguments as Variables**
  `wallWidth = 3;`
  `wallHeight + 5;`
  `getArea(wallWidth, wallHeight);`