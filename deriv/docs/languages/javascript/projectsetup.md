# Create a project

We are going to create a simple `HTML` page that contains our JavaScript file, which will handle our WebSocket connection. First, create a directory for your next project:

```
mkdir deriv-websocket-demo
```

Navigate to the `deriv-websocket-demo` folder:

```
cd deriv-websocket-demo
```

Next, create the required files as you see below:

```
touch index.html index.css index.js
```

> **TIP**
We suggest using Visual Studio Code with Live Server Extension enabled. This will help you a lot with implementations.

Now, open the `index.html` file or use the Live Server Extension.

Now, change the content of the files using the following approach:

```
index.js
console.log('we will create our websocket connection here');
```

```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Deriv HTML JS Demo</title>
  </head>
  <body>
    <h2>Deriv WebSocket API demo</h2>
    <script src="index.js" async defer />
  </body>
</html>
```

After adding the content, we can run the application by simply executing the `index.html` file or by using the Live Server Extension. When running your app, see in the console if the `console.log` is appearing. Then you know that the JavaScript file is working so that the websocket connection can be implemented properly.

For setting up the Deriv websocket, you can proceed to the WebSocket connection page.
