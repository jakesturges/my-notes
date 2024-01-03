# Flexbox

layout model that utlizies two axes which allows devs to make web-sites responsive

### `display: flex;`

- affects the children of whatever container you set to flex
- container stays at block level



```css
div.container {
    display: flex;
}
```
![Alt text](<../images/Screenshot 2024-01-02 at 4.37.17 PM.png>)
---

### `display: inline-flex;`

- changes the parent container from block level to flex


```css
div.container {
    display: inline-flex;
}
```

 ![Alt text](<../images/Screenshot 2024-01-02 at 4.44.07 PM.png>)
---

## Axis properties

### position items on main axis  
1. `justfiy-content`
2. `flex-wrap`
3. `flex-grow`
4. `flex-shrink`

### position items on cross axis
1. `align-items`
2. `align-content`

### `flex-direction`
- switches the main axis and cross axis

```css
div.container {
    display: flex;
    flex-direction: row; /* default; elements positioned from right to left */

    flex-direction: row-reverse; /* elements positioned from left to right */

    flex-direction: column; /* switches the axis; justify-content & align-items switch  */

     flex-direction: column-reverse; /* same as column but element position is reversed */
}

```