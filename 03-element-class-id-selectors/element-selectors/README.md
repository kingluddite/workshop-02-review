# Element Selectors

## Review Slide 7

## Another Example

Let's say you have an HTML file with a list of M. Night Shyamalan films, and you want to apply a specific style using CSS element selectors. Here's an example:

**index.html:**

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>M. Night Shyamalan Films</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <h1>M. Night Shyamalan Films</h1>

    <ul>
      <li>The Sixth Sense</li>
      <li>Unbreakable</li>
      <li>Signs</li>
      <li>The Village</li>
      <li>Split</li>
      <li>Glass</li>
    </ul>
  </body>
</html>
```

**styles.css:**

```css
/* Apply style to all list items within an unordered list */
ul li {
  font-family: "Arial", sans-serif;
  color: #333;
  padding: 5px;
  margin: 5px;
  background-color: #f0f0f0;
  border-radius: 5px;
}
```

In this example, the CSS element selector `ul li` targets all `<li>` elements that are descendants of a `<ul>` element. The styles applied include setting the font family, text color, padding, margin, background color, and border radius.

Feel free to customize the styles based on your preferences. When you open the HTML file in a browser, you should see a list of M. Night Shyamalan films with the specified styles applied.
