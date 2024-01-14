# id Selectors

## Review Slide 9

## Another Example

Let's create an example with an HTML file listing famous Philly cheesesteak places and use the CSS ID selector to apply specific styles to an element with a unique identifier.

**index.html:**

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Famous Philly Cheesesteak Places</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <h1>Famous Philly Cheesesteak Places</h1>

    <ul>
      <li id="genos">Geno's Steaks</li>
      <li id="pats">Pat's King of Steaks</li>
      <li id="jims">Jim's Steaks</li>
    </ul>

    <p id="cheesesteak-info">
      Discover the best cheesesteak spots in Philadelphia.
    </p>
  </body>
</html>
```

**styles.css:**

```css
/* Apply style to the element with the ID 'genos' */
#genos {
  color: #ff6600;
  font-weight: bold;
}

/* Apply style to the element with the ID 'pats' */
#pats {
  color: #009933;
  font-style: italic;
}

/* Apply style to the element with the ID 'jims' */
#jims {
  color: #ff3399;
}

/* Apply style to the element with the ID 'cheesesteak-info' */
#cheesesteak-info {
  font-size: 16px;
  color: #333;
}
```

In this example:

- Each list item (`<li>`) representing a Philly cheesesteak place has a unique ID ("genos", "pats", "jims").
- The paragraph (`<p>`) with ID "cheesesteak-info" provides general information about cheesesteaks.

The styles in the CSS file use the ID selectors (`#genos`, `#pats`, `#jims`, and `#cheesesteak-info`) to apply specific styles to elements with those unique identifiers.

Feel free to customize the styles based on your design preferences. When you open the HTML file in a browser, you should see a list of Philly cheesesteak places with different styles applied based on their IDs.
