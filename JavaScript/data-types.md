# Primitive vs Non-Primitive Data Types

## Primitive Data Types:

    - booleans, numbers, srtrings

Primitive types are part of the JavaScript language and are immutable, they can't be changed

Primitive values are "value types", the data is stored directly in the variable in memory

- stored in the stack

When they are passed into functions a new copy of that variable is made, so the original variable is unaffected

- pass-by-value

## Non Primitive Data Types:

    - objects, arrays, functions

Non-Primitve Data types are mutable, they change be changed by functions

Because an object can change at any time, the amount of memory it takes up is dynamic

Objects are stored in the Stack but their Key Value pairs / propeties live in an area of the computers memory called the Heap

- The heap can handle an objects customizability and dynamic size
- an object variable references the properties position in memory
- pass-by-refernece

 <br>

These types are also known as reference types:

- when you assign a variable to an object, it referes to that objects location in memory

### To Recap

Variables representing primitive types like numbers, strings, and booleans store information by value.<br>

When these variables are assigned to other variables or as arguments to functions, a new copy of the value is created.<br>

If modifications are made to the copied-to variable's value, it does not affect the original variable.<br>

---

Variables representing complex structures like arrays and objects store information by reference to a memory location.<br>

When these variables are assigned to other variables or as arguments to functions, a copy of the reference is created.<br>

If modifications are made to the copied-to variable's elements or properties, it also affects the original variable since the references are shared.
