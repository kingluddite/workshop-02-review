# 02 Adding CSS Three ways

Below are three ways you can add CSS to an HTML document using Rocky movie facts as the content. For simplicity, I'll provide a basic HTML structure with inline, internal, and external CSS examples.

### 1. Inline CSS (within HTML tags):

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Rocky Movie Facts</title>
  </head>
  <body
    style="background-color: #f0f0f0; font-family: Arial, sans-serif; text-align: center;"
  >
    <h1 style="color: #cc0000;">Rocky Movie Facts</h1>

    <p style="font-size: 18px; color: #333;">
      Rocky is a series of American boxing sports-drama films.
    </p>

    <!-- Add more content and styling as needed -->
  </body>
</html>
```

### 2. Internal CSS (within the `<style>` tag in the head):

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Rocky Movie Facts</title>

    <style>
      body {
        background-color: #f0f0f0;
        font-family: Arial, sans-serif;
        text-align: center;
      }

      h1 {
        color: #cc0000;
      }

      p {
        font-size: 18px;
        color: #333;
      }
    </style>
  </head>
  <body>
    <h1>Rocky Movie Facts</h1>

    <p>Rocky is a series of American boxing sports-drama films.</p>

    <!-- Add more content and styling as needed -->
  </body>
</html>
```

### 3. External CSS (separate CSS file):

**index.html:**

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Rocky Movie Facts</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <h1>Rocky Movie Facts</h1>

    <p>Rocky is a series of American boxing sports-drama films.</p>

    <!-- Add more content and styling as needed -->
  </body>
</html>
```

**styles.css:**

```css
body {
  background-color: #f0f0f0;
  font-family: Arial, sans-serif;
  text-align: center;
}

h1 {
  color: #cc0000;
}

p {
  font-size: 18px;
  color: #333;
}
```

Choose the method that best fits your project requirements and organization preferences. External CSS is generally recommended for larger projects as it allows for better organization and reusability of styles.
