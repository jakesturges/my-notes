# What is an Object?

- a container used to store data and functionality
- objects are declared and then filled with Properties(key - value pairs)
  - key names with a space are put in ' '
  - seperate key value pairs with a ,

### Object Literal Declaration

```javascript
let spaceShip = {
    'Fuel type' = 'diesel',
    color = 'silver'
};

```

### Accessing and Changing Object Properties

1. Dot notation - use for keys w / no space
   `spaceShip.color = gold;`
   <br>
   <br>
2. Bracket notation - use for keys w / spaces
   `spaceShip['Fuel Tye'] = coal;`
   - allows you to access a property of an object using a variable or an expressiom
     ```js
     const person = {
     name: 'John',
     age: 30
     };

const propertyName = 'name';
console.log(person[propertyName]); // Output: John

````

   <br>
   <br>
   <br>
   <br>

# What is a Method?

- A method is an object that has a function stored as its data
- a method is what an object does

### Example

1. `console` is an object while `.log()` is a method for that object
   <br>
   <br>
2. `Math` is an object while `.random()` and `.floor()` are methods

### Working Example

```javascript
const alienShip = {
  inavde() {
    console.log(
      "Hello! We have come to dominate your planet. Instead of Earth, it shall be called New Xaculon."
    );
  }, // methods are seperated by a ,
  takeOff() {
    console.log('Spim... Borp... Glix... Blastoff!');
  };
};

alienShip.invade(); //calling the invade() method
````
