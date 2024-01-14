# Grouping Selectors

Let's use the example of the Philly Mummers Parade and explore how advanced selectors and grouping selectors work in CSS.

### HTML Content:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Philly Mummers Parade</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <section id="comic-division">
      <h2 class="division-title">Comic Division</h2>
      <ul class="mummers-list">
        <li class="mummer">String Band 1</li>
        <li class="mummer">Comic Club 1</li>
      </ul>
    </section>
    <section id="fancy-division">
      <h2 class="division-title">Fancy Division</h2>
      <ul class="mummers-list">
        <li class="mummer">String Band 2</li>
        <li class="mummer">Fancy Brigade 1</li>
      </ul>
    </section>
  </body>
</html>
```

### CSS Styles:

```css
/* Basic Selector */
.division-title {
  font-size: 24px;
  color: #0066cc;
}

/* Grouping Selectors for Common Styles */
.mummer, .division-title {
  margin: 10px;
  padding: 8px;
  border: 1px solid #ccc;
}

/* Advanced Selectors */
#comic-division .mummer {
  background-color: #ffcc00;
}

#fancy-division .mummer {
  background-color: #ff66b2;
}
```

In this example:

- The `.division-title` class is a common style for division titles.
- The `.mummer` class is a common style for individual mummers.
- Grouping selectors are used to apply common styles to both `.mummer` and `.division-title`.

Advanced selectors using IDs and class combinations are employed to style mummers within specific divisions:

- `#comic-division .mummer`: Styles mummers within the Comic Division with a yellow background.
- `#fancy-division .mummer`: Styles mummers within the Fancy Division with a pink background.

The CSS grouping selectors and advanced selectors allow you to efficiently style common elements while also applying specific styles to elements within certain contexts. This helps maintain a clean and organized stylesheet.
