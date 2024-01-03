# Flexbox Properties 

### `justify-content:`

- positions items along the main axis (left to right )

```css
div.container {
    justify-content: flex-start;
    justify-content: flex-end;
    justify-content: center;
    justify-content: space-around;
    justify-content: space-between;
}
```

![Alt text](<../images/Screenshot 2024-01-02 at 5.18.41 PM.png>)
![Alt text](../images/image.png)
---

### `align-items:`

- positions items along the cross axis (vertical)
- used for aligning items elements whithin a single row

```css
div.container {
    align-items: flex-start;
    align-items: flex-end;
    align-items: center;
    align-items: baseline; /* bottom of content will be aligned */
}
```
![Alt-text](../images/image-1.png)
![Alt text](../images/image-2.png)

## `align-content:`

- used to align elements within a flex container that contains more than one row
- same syntax and values as `align-items:`