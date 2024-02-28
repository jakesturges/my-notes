# Short Circuit Evaluation

- can be used to replaced JS if...else statements

### Example

- if...else statement

```JavaScript
let username = '';
let defaultName;

if (username) {
    defaultName = username;
} else {
    defaultName = 'Stranger';
}

console.log(defualtName) //Prints: Stranger
```

<br>
<br>

- short circuit

```js
let username = "";
let defaulNname = username || "Stranger";

console.log(defaultName); // Prints: Stranger
```
