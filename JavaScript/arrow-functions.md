# Arrow Functions

- removes the need to type out the keyword `function`
- Syntax: `const functionName = (param1, param2) => {}`

### Example

```js
const rectangleArea = (width, height) => {
  let area = width * height;
  return area;
};
```

## Concise Body Arrow Functions

1. Functions that take only a single parameter do not need the parameter enclosed in paranthese

2. If a function takes zero or multiple parameters parantheses are required
   <br>
   <br>

ZERO PARAMETERS

```js
const functionName = () => {};
```

ONE PARAMETER

```js
const functionName = (param1) => {};
```

MULTIPLE PARAMETERES

```js
const functionName = (param1, param2) => {};
```

3. Functions with a single line body do not need curly braces and the return statement can be removed
   - this is called _implicit return_

<br>
SINGLE-LINE BODY

```js
const sumNumbers = (number) => number + number;
```
