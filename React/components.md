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
