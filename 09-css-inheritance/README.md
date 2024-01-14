# 09 CSS Inheritance

**CSS Inheritance:**

In CSS, inheritance is a mechanism where certain properties of an element are passed down to its descendants. When a property is set on a parent element, it can automatically apply to its children, simplifying the style declaration process.

Not all CSS properties are inherited; some are, by default, and others are not. For example, properties like `color`, `font-family`, and `line-height` are inherited, while properties like `margin`, `padding`, and `border` are not.

**Example with Philly Flyers HTML Content:**

Let's consider a scenario where we have a list of Philadelphia Flyers players, and we want to apply a common font family to all the players. In this example, we'll leverage the inheritance property of `font-family`.

### HTML Content:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Philly Flyers Players</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <ul class="player-list">
      <li class="player">Claude Giroux</li>
      <li class="player">Sean Couturier</li>
      <li class="player">Travis Konecny</li>
    </ul>
  </body>
</html>
```

### CSS Styles:

```css
/* Set a common font family for the body element, which will be inherited by its descendants */
body {
  font-family: "Arial", sans-serif;
}

/* Style individual player names */
.player {
  padding: 10px;
  margin: 5px;
  border: 1px solid #ccc;
}
```

In this example:

- The `font-family` property is set on the `body` element with the value `'Arial', sans-serif`.
- The player names are styled with padding, margin, and a border, but the `font-family` property is not explicitly set for them.

Due to the inheritance property of `font-family`, the common font family specified on the `body` element is automatically inherited by its descendants, including the player names. As a result, all the player names will have the specified font family.
