# Default Parameters

- allow parameters to have a predetermined value in case the function is called when no argument is passed
- use the `=` operator to assign the parameter a defualt value

### Example

```js
function greeting(name = "Stranger") {
  console.log(`Hello, ${name}!`);
}

greeting(Jake); //Prints: Hello, Jake!
greeting(); //Prints: Hello, Stranger
```
