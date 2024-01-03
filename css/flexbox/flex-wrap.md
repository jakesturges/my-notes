# `flex-wrap:`

- sets an item to be fixed to one line or allowed to span multiple lines when needed
- applied to parent container

### Values:

```css
div.container {
    display: flex;
    flex-wrap: wrap; /* child elements of a flex container that doesn't fit in a row will be pushed to the next line */

    flex-wrap: wrap-reverse; /* same as wrap value but item order is reversed */

    flex-wrap: nowrap; /* default value; prevents items from wrapping */
}

div.item {
    width: 50px;    
}

```

![Alt text](<../images/Screenshot 2024-01-02 at 8.29.53 PM.png>)