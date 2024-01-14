# 11 Node Npm

## Step 1: Create a Project Folder

Create a new folder for your project. Open a terminal or command prompt, navigate to the folder, and run the following command to initialize a new Node.js project:

```bash
npm init -y
```

## Step 2: Install Bootstrap and http-server Locally

Run the following commands to install Bootstrap and `http-server` as local dependencies:

```bash
npm install bootstrap
npm install http-server --save-dev
```

The `--save-dev` flag indicates that `http-server` is a development dependency and will be listed in the `devDependencies` section of your `package.json` file.

## Step 3: Create HTML File

Create a simple HTML file in your project folder. Let's name it `index.html`. Open it with a text editor and include the following content:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link
      rel="stylesheet"
      href="node_modules/bootstrap/dist/css/bootstrap.min.css"
    />
    <title>Node.js + Bootstrap Example</title>
  </head>
  <body>
    <div class="container">
      <h1>Hello, Bootstrap!</h1>
      <p>This is a simple example using Node.js to install Bootstrap.</p>
    </div>
    <script src="node_modules/bootstrap/dist/js/bootstrap.bundle.min.js"></script>
  </body>
</html>
```

## Step 4: Run the Local Server

Now, you can use the locally installed `http-server` to serve your HTML file. In your terminal, run the following command:

```bash
npx http-server
```

This command uses `npx` to run `http-server` without having it installed globally. Open your browser and go to the provided URL (usually `http://localhost:8080`). You should see a simple webpage styled with Bootstrap.

Using `http-server` locally ensures that it is specific to your project and does not affect the global environment. It's a common practice to include development tools as local dependencies in a project.
