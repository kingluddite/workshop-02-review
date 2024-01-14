# 05 CSS Shorthand Properties

## Review Slide 11,12,13,14,15

## Another Example

Let's create an example using the styles for two Philadelphia sports teams, the Philadelphia Eagles (football) and the Philadelphia Phillies (baseball). We'll first use longhand CSS properties and then demonstrate the equivalent styles using shorthand properties.

### Longhand CSS Properties Example:

**index.html:**

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Philly Sports Teams</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <h1>Philly Sports Teams</h1>

    <div class="team" id="eagles">
      <h2>Philadelphia Eagles</h2>
      <p>Football Team</p>
    </div>

    <div class="team" id="phillies">
      <h2>Philadelphia Phillies</h2>
      <p>Baseball Team</p>
    </div>
  </body>
</html>
```

**styles.css:**

```css
/* Style for the overall body */
body {
  font-family: "Arial", sans-serif;
  background-color: #f0f0f0;
  text-align: center;
}

/* Style for the heading */
h1 {
  color: #0066cc;
  margin-bottom: 20px;
}

/* Style for the teams */
.team {
  background-color: #fff;
  border: 2px solid #ccc;
  border-radius: 8px;
  padding: 20px;
  margin: 20px;
}

/* Style for team headings */
.team h2 {
  color: #cc0033;
  font-size: 24px;
}

/* Style for team descriptions */
.team p {
  color: #333;
}
```

### Shorthand CSS Properties Example:

**index.html:**

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Philly Sports Teams</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <h1>Philly Sports Teams</h1>

    <div class="team" id="eagles">
      <h2>Philadelphia Eagles</h2>
      <p>Football Team</p>
    </div>

    <div class="team" id="phillies">
      <h2>Philadelphia Phillies</h2>
      <p>Baseball Team</p>
    </div>
  </body>
</html>
```

**styles.css:**

```css
/* Style for the overall body */
body {
  font-family: "Arial", sans-serif;
  background-color: #f0f0f0;
  text-align: center;
}

/* Style for the heading */
h1 {
  color: #0066cc;
  margin-bottom: 20px;
}

/* Style for the teams using shorthand properties */
.team {
  background: #fff;
  border: 2px solid #ccc;
  border-radius: 8px;
  padding: 20px;
  margin: 20px;
}

/* Style for team headings */
.team h2 {
  color: #cc0033;
  font-size: 24px;
}

/* Style for team descriptions */
.team p {
  color: #333;
}
```

In the shorthand example, we've used the `background` shorthand property instead of specifying `background-color`. Additionally, we've utilized the `border`, `border-radius`, and `margin` properties in shorthand form. Note that in some cases, using shorthand properties can make the code more concise and easier to read. However, it's essential to strike a balance between brevity and readability based on your coding preferences and team conventions.

## The CSS Border

Let's create an example using the CSS `border` property, both the longhand and shorthand versions.

### Longhand CSS `border` Property Example:

```css
/* Longhand Properties */
.example-longhand {
  border-width: 2px;
  border-style: dashed;
  border-color: #ff6600;
}
```

### Shorthand CSS `border` Property Example:

```css
/* Shorthand Property */
.example-shorthand {
  border: 2px dashed #ff6600;
}
```

In the longhand example, each aspect of the `border` property (width, style, and color) is specified separately using the longhand properties `border-width`, `border-style`, and `border-color`.

In the shorthand example, all three properties are combined into a single `border` property. The values are provided in the order of `width`, `style`, and `color`.

Both examples achieve the same result—a dashed border with a width of 2 pixels and an orange color. The choice between longhand and shorthand depends on your preference for readability and how you prefer to organize your CSS code. Shorthand can be more concise, while longhand may provide clarity in some situations.

## The CSS font property

Certainly! Let's create an example using the CSS `font` property, both the longhand and shorthand versions.

### Longhand CSS `font` Property Example:

```css
/* Longhand Properties */
.example-longhand {
  font-style: italic;
  font-weight: bold;
  font-size: 16px;
  line-height: 1.5;
  font-family: "Arial", sans-serif;
  color: #333;
}
```

### Shorthand CSS `font` Property Example:

```css
/* Shorthand Property */
.example-shorthand {
  font: italic bold 16px/1.5 "Arial", sans-serif;
  color: #333; /* additional properties can be added separately */
}
```

In the longhand example, each aspect of the `font` property (style, weight, size, line height, family) is specified separately using the longhand properties `font-style`, `font-weight`, `font-size`, `line-height`, and `font-family`.

In the shorthand example, all these properties are combined into a single `font` property. The values are provided in the order of `font-style`, `font-weight`, `font-size`, `line-height`, and `font-family`.

Both examples achieve the same result—italic, bold text with a font size of 16 pixels, a line height of 1.5, using the 'Arial' font family, and a color of #333. The choice between longhand and shorthand depends on your coding style and how you prefer to structure your CSS. Shorthand can be more concise, while longhand may provide explicit clarity in some situations.

## The CSS Background Property

Certainly! Let's create an example using the CSS `background` property, both the longhand and shorthand versions.

### Longhand CSS `background` Property Example:

```css
/* Longhand Properties */
.example-longhand {
  background-color: #f0f0f0;
  background-image: url("example-image.jpg");
  background-repeat: no-repeat;
  background-position: center top;
  background-size: cover;
}
```

### Shorthand CSS `background` Property Example:

```css
/* Shorthand Property */
.example-shorthand {
  background: #f0f0f0 url("example-image.jpg") no-repeat center top / cover;
}
```

In the longhand example, each aspect of the `background` property (color, image, repeat, position, size) is specified separately using the longhand properties `background-color`, `background-image`, `background-repeat`, `background-position`, and `background-size`.

In the shorthand example, all these properties are combined into a single `background` property. The values are provided in the order of `background-color`, `background-image`, `background-repeat`, `background-position`, `background-size`. Additionally, the `/` separates the background position and size.

Both examples achieve the same result—a background with a color of #f0f0f0, an image ('example-image.jpg') positioned at the center top, not repeated, and covering the background. The choice between longhand and shorthand depends on your coding style and how you prefer to structure your CSS. Shorthand can be more concise, while longhand may provide explicit clarity in some situations.

# Should I always use shorthand css properties?

Using shorthand CSS properties can be beneficial for writing more concise and readable code, but whether you should always use them depends on the context, your coding style, and the requirements of your project. Here are some considerations:

### Advantages of Shorthand CSS Properties:

1. **Conciseness:** Shorthand properties allow you to express multiple related values in a single line, making your CSS more compact and easier to scan.

2. **Readability:** In many cases, shorthand properties can improve code readability, especially when dealing with commonly grouped properties like `margin`, `padding`, `border`, and `background`.

3. **Maintenance:** Shorthand properties can simplify maintenance by reducing the number of lines you need to update when making changes to related styles.

### Considerations and Best Practices:

1. **Understanding:** Ensure that you and your team have a clear understanding of shorthand properties and their syntax to avoid confusion.

2. **Specificity:** Be aware that using shorthand properties might override more specific styles if not used carefully. For instance, using `border` might override specific `border-width` or `border-color` styles.

3. **Consistency:** Consistency in your codebase is crucial. If your team has a coding style guide, follow it to maintain a uniform and readable codebase.

4. **Complex Styles:** For more complex styles or when applying styles conditionally, it might be clearer to use longhand properties.

5. **Performance:** In terms of performance, the impact of using shorthand properties vs. longhand properties is negligible. Choose based on code clarity and maintainability rather than performance considerations.

### Example:

```css
/* Longhand Properties */
padding-top: 10px;
padding-right: 20px;
padding-bottom: 10px;
padding-left: 20px;

/* Shorthand Property */
padding: 10px 20px;
```

In this example, both sets of code achieve the same result, but the shorthand version is more concise.

### Conclusion:

While shorthand properties can be advantageous, it's essential to strike a balance and use them where they enhance code clarity. Consistency within your team and adherence to coding standards are crucial. Consider readability and maintainability as primary factors when deciding whether to use shorthand or longhand properties in your CSS.
