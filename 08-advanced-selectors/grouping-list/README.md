# Grouping List

Let's consider a scenario where you have an HTML document with a list of items grouped into different categories, and you want to apply different styles to items within each category using CSS advanced selectors.

### HTML Content:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Grouping List - CSS Advanced Selectors</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <ul class="category-list" id="fruits">
      <li class="item">Apple</li>
      <li class="item">Banana</li>
      <li class="item">Orange</li>
    </ul>

    <ul class="category-list" id="vegetables">
      <li class="item">Carrot</li>
      <li class="item">Broccoli</li>
      <li class="item">Tomato</li>
    </ul>

    <ul class="category-list" id="desserts">
      <li class="item">Chocolate Cake</li>
      <li class="item">Ice Cream</li>
      <li class="item">Cheesecake</li>
    </ul>
  </body>
</html>
```

### CSS Styles:

```css
/* Common styles for items */
.item {
  padding: 8px;
  margin: 8px;
  border: 1px solid #ccc;
}

/* Advanced selectors for specific categories */
#fruits .item {
  background-color: #ffcc99; /* Light orange */
}

#vegetables .item {
  background-color: #ccffcc; /* Light green */
}

#desserts .item {
  background-color: #ffd9b3; /* Light brown */
}
```

In this example:

- Each `<ul>` element represents a category list (`fruits`, `vegetables`, `desserts`).
- Each `<li>` element within the lists has a class of `item`.
- The common styling for items (padding, margin, border) is applied using the `.item` selector.
- Advanced selectors with IDs are used to apply specific background colors to items within each category.

With these CSS rules, items in the "fruits" category will have a light orange background, items in the "vegetables" category will have a light green background, and items in the "desserts" category will have a light brown background.
