# Components: UI building blocks

- lets you combine html, css, and JS into custom "Components"
- these Componets are **resuable UI elements for your app**
- They are regular javascript functions except:
  1. Their names begin with Capital letter

### Example of Page Made Using Components

```js
<PageLayout>
  <NavigationHeader>
    <SearchBar />
    <Link to="/docs">Docs</Link>
  </NavigationHeader>
  <Sidebar />
  <PageContent>
    <TableOfContents />
    <DocumentationText />
  </PageContent>
</PageLayout>
```

In the above exaxmple the `<TableOfContents/>` component may look like this under the hood:

```html
<article>
  <h1>My First Component</h1>
  <ol>
    <li>Components: UI Building Blocks</li>
    <li>Defining a Component</li>
    <li>Using a Component</li>
  </ol>
</article>
```

## Defining a Component

### Example

```js
// module.js
export default function Profile() {
  return <img src="https://i.imgur.com/MK3eW3Am.jpg" alt="Katherine Johnson" />;
}
```

### Step 1: Export the component

- use `export default`
- used to export a single function, value, or object from a js file
  - a file can only have one default export
- In the above example the defualt export for module.js is the `Profile()` function
  - whenever you import this file into another file it will get the value assigned to `Profile()`

### Step 2: Define the function

- in the ex `function Profile() {}` was defined

### Step 3: Add markup

- in this case the markup is an `<imng>`tag

## Using a Component

The `Profile` component can be used individualy or nested inside other components. In the example below we can export the `Gallery` component which has multiple `Profile` components nested whithin.

```js
function Profile() {
  return <img src="https://i.imgur.com/MK3eW3As.jpg" alt="Katherine Johnson" />;
}

export default function Gallery() {
  return (
    <section>
      <h1>Amazing scientists</h1>
      <Profile />
      <Profile />
      <Profile />
    </section>
  );
}
```

## Exporting and Importing a Component

A component can be moved in 3 steps:

1. Make a new js file to put components into
2. Use `export default` to export the function component
3. Import the component to into the file you will use it in

Example:

```js
//App.js
import Gallery from './Gallery.js';

export default function App() {
  return (
    <Gallery />
  );
}

//Gallery.js
function Profile() {
  return (
    <img
      src="https://i.imgur.com/QIrZWGIs.jpg"
      alt="Alan L. Hart"
    />
  );
}

export default function Gallery() {
  return (
    <section>
      <h1>Amazing scientists</h1>
      <Profile />
      <Profile />
      <Profile />
    </section>
  );
}
```

- as you can see the `Gallery()` & `Profile()` components were placed into a seperate Gallery.js file
- in App.js (root component file) the components were imported with `import` method

1. `Gallery.js`:
   - `Profile()` component is used within same file but not exported
   - `Gallery()` component is set as default export

## Exporting and Importing Multiple Components From Same File

- use named exports
- as previously stated, a file can only have 1 defualt export but it can have multiple named exports

### Syntax Export:

- just remove default keyword

```js
export function Profile() {
  //code
}
```

### Syntax Import:

- place named export within curly braces

```js
import { Profile } from "./Gallery.js"; //importing named export
import Gallery from "./Gallery.js"; // importing default export
```
