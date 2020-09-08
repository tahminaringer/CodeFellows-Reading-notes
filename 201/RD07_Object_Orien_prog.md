# Read 07 Object Oriented Programing

## Domain Modeling

-Concept of creating a conceptual model in code for a specific problem.
  - Describes the entities, attributes, behaviors and contraints that govern the problem domain.
  - **Object Oriented** Entity that stores data in properties and encapsulates behaviors in methods

### Tips for Building Domain Models

1. When modeling a single entity that'll have many instances, build self-contained objects with the same attributes and behaviors.
2. Model its attributes with a constructor function that defines and initializes properties.
3. Model its behaviors with small methods that focus on doing one job well.
4. Create instances using the new keyword followed by a call to a constructor function.
5. Store the newly created object in a variable so you can access its properties and methods from outside.
6. Use the this variable within methods so you can access the object's properties and methods from inside.

## HTML Chapter 6 Tables

- **Table** Represents something in a grid format.
  - `<table>` creates table
  - `<tr>`indicates the start of each row/ contains all the cell data
  - `<td>` represents each cell of the table, match amount of trs 
  - `<th>` represents the heading for either a column or a row
- **Spanning columns** use `calspan=""` attribute
- **Spanning Rows** use ` rowspan=""`
-**Long Tables**
  - `<thead>` heading of the table
  - `<tbody>` the body of the table
  - `<tfoot>` the footer of the table

## JS Chapter 3 Functions, Methods & Objects

- **Update the value of properties** Use dot notation or square brackets.

```ex
hotel.name = 'park';
hotel['name'] = 'park';
```

- **Global Scope/global context** when a function is created at the top level of a script
- `this` used inside functions and objects. this referes to on object, usually the object in which the function operates.
- **Object model** is a greoup of objects each of which represent related things from the real world.
- **Browser Object Model** creates a model of the browser tab or window.
- **Document Object Model** creates a model of the current web page
- **Global JS Objects** group of individual objects that relate to different parts of the JS language.
- **Global Objects:String object** when you have a value that is a string , you can use the properties and methods of the string object on that value.
- **Simple/Primitive data types** string, number boolean, undefined, null.
- **Complex Data Type** is an object
- **Global Objects: number Objects** whenever you have a value that is a number, you can use the methods and properties of the number object on it.
- **Global Math Object** The Math object has properities and methods for mathmatical constants and functions
- **Date Object/Time** Once you have created a Date object, the following methods let you set and retrieve the time and date that it represents.

