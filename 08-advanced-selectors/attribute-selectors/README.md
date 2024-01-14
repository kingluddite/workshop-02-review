## CSS Attribute Selectors

Let's consider an HTML document containing information about Philadelphia universities, and we'll use CSS attribute selectors to style specific elements based on their attributes.

### HTML Content:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Philadelphia Universities</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <h1 data-category="public">Public Universities</h1>
    <ul>
      <li data-type="university" data-rank="1">University of Pennsylvania</li>
      <li data-type="college" data-rank="2">Temple University</li>
      <li data-type="university" data-rank="3">Drexel University</li>
    </ul>

    <h1 data-category="private">Private Universities</h1>
    <ul>
      <li data-type="university" data-rank="1">Saint Joseph's University</li>
      <li data-type="college" data-rank="2">La Salle University</li>
      <li data-type="university" data-rank="3">Villanova University</li>
    </ul>
  </body>
</html>
```

### CSS Styles:

```css
/* Style all elements with data-category attribute */
[data-category] {
  font-size: 24px;
  color: #0066cc; /* Blue */
  margin-bottom: 10px;
}

/* Style specific elements with data-type and data-rank attributes */
[data-type="university"][data-rank="1"] {
  font-weight: bold;
  color: #cc3300; /* Red */
}

[data-type="college"][data-rank="2"] {
  font-style: italic;
  color: #009933; /* Green */
}
```

In this example:

- `<h1>` elements have a `data-category` attribute to categorize the universities as "public" or "private."
- `<li>` elements have `data-type` and `data-rank` attributes to specify the type (university or college) and the rank of the institution.
- CSS attribute selectors are used to apply styles to elements based on their attributes.

With these CSS rules:

- All elements with the `data-category` attribute will have a blue color and a larger font size.
- Elements with `data-type="university"` and `data-rank="1"` will have bold text and a red color.
- Elements with `data-type="college"` and `data-rank="2"` will have italic text and a green color.

These attribute selectors provide a way to target specific elements based on their attributes, allowing for more granular styling based on the content and structure of the HTML.
