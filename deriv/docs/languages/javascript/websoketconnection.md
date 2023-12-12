# WebSocket connection

Next, we'll create a WebSocket connection to Deriv WebSocket Server as seen below:

const app_id = 1089; // Replace with your app_id or leave as 1089 for testing.
const websocket = new WebSocket(`wss://ws.derivws.com/websockets/v3?app_id=${app_id}`);

> **INFO**
`app_id = 1089` is just for testing purposes. Please update it with your own app_id when releasing your application on a production environment. Please check this guide to create a new app for yourself.

At this point, we are connected to the `WebSocket server`. But, we do not receive any data. To send or receive data, we have to `subscribe` to websocket events.

Generally, we have 4 events on `WebSocket connections`:

* **close:** Fired when a connection with a WebSocket is closed. Also available via the onclose property.
* **open:** Fired when a connection with a WebSocket is opened. Also available via the onopen property.
* **message:** Fired when data is received through a  WebSocket. Also available via the onmessage property.
* **error:** Fired when a connection with a WebSocket has been closed because of an error, such as when some data couldn't be sent. Also available via the onerror property.

Let's add an event listener for these events on our WebSocket connection.
