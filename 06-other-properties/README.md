# Other Properties

## CSS Display

Review Slide 16

## Other Example

Let's use the CSS `display` property to style facts about the Liberty Bell with different display values: `block`, `inline`, and `inline-block`.

### Block Display Example:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Liberty Bell Facts</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <div class="fact-block">
      <h2>Liberty Bell</h2>
      <p>
        The Liberty Bell is an iconic symbol of American independence located in
        Philadelphia, Pennsylvania.
      </p>
      <p>
        It is inscribed with the words "Proclaim LIBERTY Throughout all the Land
        unto all the Inhabitants Thereof."
      </p>
      <p>The bell weighs about 2,080 pounds and has a crack.</p>
    </div>
  </body>
</html>
```

```css
/* Block Display Style */
.fact-block {
  display: block;
  width: 70%;
  margin: 20px auto;
  background-color: #f0f0f0;
  padding: 20px;
  border: 2px solid #ccc;
  border-radius: 8px;
  text-align: left;
}
```

In this example, the Liberty Bell facts are enclosed in a `<div>` with a class of `fact-block`, and the CSS sets `display: block` to make it a block-level element. This makes it take up the full width available and start on a new line.

### Inline Display Example:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Liberty Bell Facts</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <span class="fact-inline">
      <h2>Liberty Bell</h2>
      <p>
        The Liberty Bell is an iconic symbol of American independence located in
        Philadelphia, Pennsylvania.
      </p>
      <p>
        It is inscribed with the words "Proclaim LIBERTY Throughout all the Land
        unto all the Inhabitants Thereof."
      </p>
      <p>The bell weighs about 2,080 pounds and has a crack.</p>
    </span>
  </body>
</html>
```

```css
/* Inline Display Style */
.fact-inline {
  display: inline;
  background-color: #f0f0f0;
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 4px;
  text-align: left;
}
```

In this example, the Liberty Bell facts are enclosed in a `<span>` with a class of `fact-inline`, and the CSS sets `display: inline` to make it an inline-level element. This makes it flow within the content and not start on a new line.

### Inline-Block Display Example:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Liberty Bell Facts</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <div class="fact-inline-block">
      <h2>Liberty Bell</h2>
      <p>
        The Liberty Bell is an iconic symbol of American independence located in
        Philadelphia, Pennsylvania.
      </p>
      <p>
        It is inscribed with the words "Proclaim LIBERTY Throughout all the Land
        unto all the Inhabitants Thereof."
      </p>
      <p>The bell weighs about 2,080 pounds and has a crack.</p>
    </div>
  </body>
</html>
```

```css
/* Inline-Block Display Style */
.fact-inline-block {
  display: inline-block;
  width: 45%;
  margin: 10px;
  background-color: #f0f0f0;
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 4px;
  text-align: left;
  vertical-align: top;
}
```

In this example, the Liberty Bell facts are enclosed in a `<div>` with a class of `fact-inline-block`, and the CSS sets `display: inline-block` to make it an inline-block element. This makes it flow within the content, but unlike inline, it can have width and height properties, and it still respects box-model properties such as padding and margin.

## CSS Color Values and Color Property

### Review Slide 17

### Other Examples

Let's create examples of different CSS color values and the `color` property using the Philadelphia Phillies, the 1980 World Series winners, as the content.

### Example 1: Named Color Value

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>1980 World Series - Phillies</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <div class="phillies-info">
      <h1>1980 World Series Champions - Philadelphia Phillies</h1>
      <p>
        The Philadelphia Phillies won the 1980 World Series against the Kansas
        City Royals.
      </p>
    </div>
  </body>
</html>
```

```css
/* Named Color Value Example */
.phillies-info {
  color: red; /* Named color value */
  background-color: white;
  padding: 20px;
  text-align: center;
}
```

In this example, the text color is set to the named color value `red`, representing the Phillies' team color.

### Example 2: Hexadecimal Color Value

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>1980 World Series - Phillies</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <div class="phillies-info">
      <h1>1980 World Series Champions - Philadelphia Phillies</h1>
      <p>
        The Philadelphia Phillies won the 1980 World Series against the Kansas
        City Royals.
      </p>
    </div>
  </body>
</html>
```

```css
/* Hexadecimal Color Value Example */
.phillies-info {
  color: #ff0000; /* Hexadecimal color value for red */
  background-color: #ffffff; /* Hexadecimal color value for white */
  padding: 20px;
  text-align: center;
}
```

In this example, the text color is set using the hexadecimal color value `#ff0000` (red), and the background color is set using `#ffffff` (white).

### Example 3: RGB Color Value

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>1980 World Series - Phillies</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <div class="phillies-info">
      <h1>1980 World Series Champions - Philadelphia Phillies</h1>
      <p>
        The Philadelphia Phillies won the 1980 World Series against the Kansas
        City Royals.
      </p>
    </div>
  </body>
</html>
```

```css
/* RGB Color Value Example */
.phillies-info {
  color: rgb(255, 0, 0); /* RGB color value for red */
  background-color: rgb(255, 255, 255); /* RGB color value for white */
  padding: 20px;
  text-align: center;
}
```

In this example, the text color is set using the RGB color value `rgb(255, 0, 0)` (red), and the background color is set using `rgb(255, 255, 255)` (white).

# Which color value should I use?

The choice of color value depends on various factors, including personal preference, design requirements, and the specific use case. Here are common color value formats and considerations for choosing them:

1. **Named Colors:**

   - **Examples:** `red`, `blue`, `green`, etc.
   - **Pros:** Easy to remember and understand. Can be useful for standard colors.
   - **Cons:** Limited selection. Not suitable for custom or precise colors.

2. **Hexadecimal Colors:**

   - **Example:** `#ff0000` (red)
   - **Pros:** Wide range of colors. Precise and consistent representation.
   - **Cons:** May be less human-readable compared to named colors.

3. **RGB Colors:**

   - **Example:** `rgb(255, 0, 0)` (red)
   - **Pros:** Provides control over individual color channels. Suitable for precise adjustments.
   - **Cons:** Longer syntax compared to hexadecimal. Less commonly used directly in CSS.

4. **RGBA Colors (with Alpha Channel for Transparency):**

   - **Example:** `rgba(255, 0, 0, 0.5)` (semi-transparent red)
   - **Pros:** Allows setting transparency. Useful for overlays and gradients.
   - **Cons:** Slightly more complex syntax.

5. **HSL Colors (Hue, Saturation, Lightness):**

   - **Example:** `hsl(0, 100%, 50%)` (red)
   - **Pros:** Intuitive for adjusting color properties. Useful for creating variations.
   - **Cons:** Less commonly used. Longer syntax compared to hexadecimal.

6. **HSLA Colors (with Alpha Channel for Transparency):**
   - **Example:** `hsla(0, 100%, 50%, 0.5)` (semi-transparent red)
   - **Pros:** Combines HSL with transparency. Offers intuitive adjustments.
   - **Cons:** Longer syntax compared to hexadecimal.

### Recommendations:

- **For Standard Colors:** Named colors can be convenient and expressive (e.g., `red`, `blue`).
- **For Precise Colors:** Hexadecimal or RGB values provide precise control over color.
- **For Transparency:** Use RGBA or HSLA when transparency is required.

Ultimately, the choice depends on your specific needs and the design aesthetics of your project. In many cases, a combination of these formats may be used throughout a stylesheet based on the situation. Choose the format that aligns with your project's design goals and your personal coding style.

# Why do many developers prefer HSLA?

Many developers prefer HSLA (Hue, Saturation, Lightness, Alpha) color representation for several reasons:

1. **Intuitive Adjustments:** HSLA values provide an intuitive way to adjust color properties. Developers can easily change the hue, saturation, lightness, and alpha values to achieve different variations without dealing with complex calculations or conversions.

2. **Ease of Understanding:** The HSLA color model is more human-readable and understandable compared to RGB or hexadecimal values. The terms "hue," "saturation," and "lightness" are more descriptive of the color characteristics, making it easier for developers to work with.

3. **Color Variations:** HSLA makes it straightforward to create variations of a color by adjusting its hue, saturation, or lightness. This is particularly useful when working with color schemes or designing user interfaces where variations of a base color are needed.

4. **Transparency Control:** The "A" in HSLA stands for alpha, which represents the level of transparency. Including the alpha channel allows developers to control the opacity of the color, making it easy to create semi-transparent or fully transparent colors when needed.

5. **Consistency Across Shades:** Adjusting the lightness value in HSLA tends to produce consistent changes across various shades of a color. This is in contrast to adjusting the brightness in RGB, where changes may not be perceived uniformly.

6. **Easier to Learn:** For developers who are relatively new to working with colors in CSS, HSLA may be easier to learn and grasp initially. The separation of color properties into distinct components (hue, saturation, lightness, alpha) simplifies the understanding of how color works.

7. **CSS Preprocessors Support:** CSS preprocessors like Sass and Less often have built-in functions and utilities for working with HSLA, making it convenient for developers using these tools.

8. **Accessibility:** HSLA can contribute to improved accessibility by making it easier for developers to choose color combinations that meet accessibility standards, considering factors such as contrast and legibility.
