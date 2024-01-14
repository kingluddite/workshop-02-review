# CSS Combinators

Certainly! Let's create an example using combinators to style elements related to the times when the Philadelphia Eagles were in the Super Bowl.

### HTML Content:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Philly Eagles Super Bowl Appearances</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <section id="super-bowl-15">
      <h2>Super Bowl XV (1981)</h2>
      <ul class="appearance-details">
        <li>Opponent: Oakland Raiders</li>
        <li>Result: Loss</li>
      </ul>
    </section>

    <section id="super-bowl-39">
      <h2>Super Bowl XXXIX (2005)</h2>
      <ul class="appearance-details">
        <li>Opponent: New England Patriots</li>
        <li>Result: Loss</li>
      </ul>
    </section>

    <section id="super-bowl-52">
      <h2>Super Bowl LII (2018)</h2>
      <ul class="appearance-details">
        <li>Opponent: New England Patriots</li>
        <li>Result: Win</li>
      </ul>
    </section>
  </body>
</html>
```

### CSS Styles:

```css
/* Style section headings for Super Bowl appearances */
h2 {
  color: #004080; /* Dark blue */
}

/* Style appearance details for each Super Bowl */
.appearance-details > li {
  margin: 8px;
  padding: 8px;
  border: 1px solid #ccc;
}

/* Style Super Bowl appearances using combinators */
#super-bowl-15 + #super-bowl-39 {
  background-color: #ffcc99; /* Light orange background for consecutive appearances */
}

#super-bowl-39 ~ #super-bowl-52 {
  background-color: #b3ffb3; /* Light green background for non-consecutive appearances */
}
```

In this example:

- Each Super Bowl appearance is represented by a `<section>` element with a specific ID (`super-bowl-15`, `super-bowl-39`, `super-bowl-52`).
- Section headings (`<h2>`) are styled with a dark blue color.
- Appearance details (`<li>`) are styled with margin, padding, and a border.

Combinators are used to apply specific styles to Super Bowl appearances:

- Adjacent sibling combinator (`+`) is used to style Super Bowl XXXIX with a light orange background when it follows Super Bowl XV consecutively.
- General sibling combinator (`~`) is used to style Super Bowl LII with a light green background when it follows Super Bowl XXXIX non-consecutively.

## What does the + and ~ mean?

In CSS, the `+` and `~` symbols are combinators used to define relationships between selectors. They help you apply styles based on the position or relationship of elements within the HTML structure.

1. **Adjacent Sibling Combinator `+`:**

   - The `+` combinator selects an element that is immediately preceded by a specified element. It targets the first element that is immediately followed by another element.
   - Syntax: `element1 + element2`
   - Example: `#element1 + #element2` selects `#element2` only if it is immediately preceded by `#element1`.
   - Usage: This is useful when you want to style an element that directly follows another specific element.

2. **General Sibling Combinator `~`:**
   - The `~` combinator selects all elements that are siblings of a specified element and share the same parent. It targets all sibling elements that come after the specified element.
   - Syntax: `element1 ~ element2`
   - Example: `#element1 ~ .class2` selects all elements with class `.class2` that are siblings of `#element1`.
   - Usage: This is useful when you want to style elements that come after a specific element, regardless of their immediate relationship.

### Examples:

Let's consider the following HTML structure:

```html
<div id="element1"></div>
<div id="element2"></div>
<div class="class2"></div>
<div class="class2"></div>
```

- Using the adjacent sibling combinator (`+`):

  ```css
  #element1 + #element2 {
    /* Styles applied to #element2 immediately following #element1 */
  }
  ```

- Using the general sibling combinator (`~`):
  ```css
  #element1 ~ .class2 {
    /* Styles applied to all elements with class .class2 that follow #element1 */
  }
  ```
