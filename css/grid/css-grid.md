# CSS Grid

creates a two dimensional grid consisting of rows and columns

## Container Properties

`display: grid` - creates a grid

```css
.grid-container {
  display: grid; /* declare a grid */
  width: 400px;
  height: 300px;
}
```

`grid-template-rows` - defines number and size of rows

```css
.grid-container {
  display: grid;
  width: 400px;
  height: 300px;
  grid-template-rows: 1fr 1fr 1fr; /* creates three rows of equal length */
}
```

`grid-template-columns` - defines number and size of columns

`grid-template`

`row-gap`

`column-gap`

## Item Properties

```css
.grid-container {
  display: grid; /* declare a grid */
  width: 400px;
  height: 300px;
}

.grid-item {
}
```
