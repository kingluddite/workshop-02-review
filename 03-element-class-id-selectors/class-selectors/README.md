# Class Selectors

## Review slide 8

- The "dot" (.)
- naming syntax

Let's assume you have an HTML file listing some historical revolutionary battlefields in Pennsylvania, and you want to apply a specific style to elements with a specific class using a CSS class selector. Here's an example:

**index.html:**

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Revolutionary Battlefields in Pennsylvania</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <h1>Revolutionary Battlefields in Pennsylvania</h1>

    <ul>
      <li class="battlefield">Valley Forge</li>
      <li class="battlefield">Brandywine</li>
      <li class="battlefield">Germantown</li>
      <li class="battlefield">Trenton</li>
      <li class="battlefield">Saratoga</li>
    </ul>
  </body>
</html>
```

**styles.css:**

```css
/* Apply style to elements with the class 'battlefield' */
.battlefield {
  font-family: "Georgia", serif;
  color: #0066cc;
  font-weight: bold;
}
```

In this example, the CSS class selector `.battlefield` targets all elements with the class "battlefield" and applies the specified styles. The styles include setting the font family, text color, and font weight.

Feel free to customize the styles based on your preferences. When you open the HTML file in a browser, you should see a list of revolutionary battlefields in Pennsylvania with the specified styles applied to the elements with the "battlefield" class.

## Multiple Classes and Reused

Let's modify the example to include elements with multiple classes, and we'll reuse those classes in different parts of the document:

**index.html:**

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Revolutionary Battlefields in Pennsylvania</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <h1>Revolutionary Battlefields in Pennsylvania</h1>

    <ul>
      <li class="battlefield historical">Valley Forge</li>
      <li class="battlefield">Brandywine</li>
      <li class="battlefield historical">Germantown</li>
      <li class="battlefield">Trenton</li>
      <li class="battlefield">Saratoga</li>
    </ul>

    <p class="historical">
      Explore the rich history of these battlefields in Pennsylvania.
    </p>
  </body>
</html>
```

**styles.css:**

```css
/* Apply style to elements with the class 'battlefield' */
.battlefield {
  font-family: "Georgia", serif;
  color: #0066cc;
  font-weight: bold;
}

/* Apply style to elements with the class 'historical' */
.historical {
  font-style: italic;
  color: #333;
}
```

In this modified example:

- The list items in the `<ul>` element have both the "battlefield" and "historical" classes. The "battlefield" class provides specific styles for battlefield items, while the "historical" class adds styles related to historical content.

- The paragraph `<p>` element at the end has the "historical" class. This class is reused, demonstrating how you can apply consistent styles to different elements with the same class.

Feel free to customize the styles and classes further based on your design preferences. When you open the HTML file in a browser, you should see a list of revolutionary battlefields with different styles applied based on their classes.
