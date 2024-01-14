# 07 CSS Specificity

## Review Slide 18 - 21

## Other Examples

* [specificity calculator](https://specificity.keegan.st/)
* [CSS Specificity and When to Use the CSS Important Tag](https://www.freecodecamp.org/news/what-is-css-specificity/)

CSS specificity is a set of rules that determines which style declarations are applied to an HTML element when there are conflicting styles from different sources. Let's use the example of the Philadelphia 76ers in an HTML document to explain CSS specificity and how it applies to various sources of CSS.

### HTML Content:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Philadelphia 76ers</title>
    <link rel="stylesheet" href="external-styles.css" />
    <style>
      /* Internal Styles */
      body {
        background-color: #f0f0f0;
        font-family: "Arial", sans-serif;
      }
    </style>
  </head>
  <body>
    <h1 style="color: red;">Philadelphia 76ers</h1>
    <p class="team-description">
      The Philadelphia 76ers are a professional basketball team...
    </p>
  </body>
</html>
```

### CSS Sources:

1. **Inline Styles:**

   - Applied directly to an element using the `style` attribute.
   - Highest specificity.
   - Example: `<h1 style="color: red;">`

2. **Internal Stylesheet:**

   - Defined within the `<style>` tag in the HTML document.
   - Middle specificity.
   - Example: `body { background-color: #f0f0f0; }`

3. **External Stylesheet:**
   - Linked using the `<link>` tag with an external CSS file.
   - Lowest specificity among external styles.
   - Example: `link rel="stylesheet" href="external-styles.css"`

### CSS Specificity Rules:

The CSS specificity rules determine which styles take precedence when there are conflicting styles from different sources:

1. **Inline Styles:**

   - Highest specificity.
   - Directly applied to an element using the `style` attribute.

2. **ID Selectors:**

   - Higher specificity than class or tag selectors.
   - Example: `#element-id { ... }`

3. **Class and Attribute Selectors:**

   - Medium specificity.
   - Examples: `.class-name { ... }`, `[attribute="value"] { ... }`

4. **Type (Tag) Selectors:**
   - Lowest specificity.
   - Examples: `h1 { ... }`, `p { ... }`

### Cascading Algorithm:

The cascading algorithm in CSS determines how conflicting styles are resolved based on specificity and the order in which styles are declared. Here's a simplified explanation:

1. **Specificity:** Styles with higher specificity take precedence over those with lower specificity.
2. **Order of Declaration:** If specificity is equal, the last declared style wins.

### Example:

Let's assume there's a rule in both the internal and external stylesheets targeting the `.team-description` class:

```css
/* Internal Styles */
.team-description {
  font-weight: bold;
}

/* External Styles */
.team-description {
  font-style: italic;
}
```

In this case, the external stylesheet's rule will be applied because both rules have the same specificity, and the order of declaration favors the one declared later in the stylesheet.

Understanding CSS specificity is crucial for developers to manage and troubleshoot styles effectively, especially in larger projects where styles can come from various sources.
