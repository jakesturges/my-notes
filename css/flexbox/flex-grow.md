#  `flex-grow:`

- by default all flex items shrink if the parent container is too small but do not grow if the parent container is large
- `flex-grow:` allows us to specifiy what items should grow to fit the container
    - is applied to flex items not flex containers

    ```css
    div.container {
        display: flex;
    }

    div.item {
        flex-grow: 1;
    }
    ```



# `flex-shrink`

- by default flex items have a flex-shrink value of 1
- same syntax as flex-grow

 ```css
    div.container {
        display: flex;
    }

    div.item {
        flex-shrink: 1;
    }
```

# `flex-basis`

- allows you to specify the width of an element before it shrinks or grows 

```css
    div.container {
        display: flex;
    }

    div.item {
        flex-shrink: 1;
        flex-basis: 50px; /* the width of div.item is set to 50px */
    }
```

# ` flex:`

- allows you to declare `flex-grow`, `flex-shrink`, and `flex-basis` on the same line

```css

div.container {
    display: flex;
}

div.item {
    flex: 1 2 60px; /* here flex-grow = 1, flex-shrink = 2, & flex-basis = 60px */
}

```