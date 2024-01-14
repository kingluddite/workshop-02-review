# Pseudo Classes

Let's use pseudo-classes to style elements related to famous Philadelphia actors based on user interactions. In this example, we'll apply styles when the user hovers over the actor names.

### HTML Content:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Famous Philly Actors</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <ul class="actor-list">
      <li class="actor">Will Smith</li>
      <li class="actor">Kevin Hart</li>
      <li class="actor">Meryl Streep</li>
    </ul>
  </body>
</html>
```

### CSS Styles:

```css
/* Define the default styles for actor names */
.actor {
  padding: 10px;
  margin: 5px;
  border: 1px solid #ccc;
}

/* Apply styles when the user hovers over actor names */
.actor:hover {
  background-color: #ffcc99; /* Light orange background on hover */
  color: #cc3300; /* Dark orange text color on hover */
  cursor: pointer; /* Change cursor to pointer on hover */
}
```

In this example:

- Each actor's name is represented by an `<li>` element with the class `actor`.
- The default styles for actor names include padding, margin, and a border.
- The `:hover` pseudo-class is used to apply styles when the user hovers over an actor's name. On hover, the background color changes to light orange, the text color changes to dark orange, and the cursor changes to a pointer.
