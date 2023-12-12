# What are WebSockets?

The `WebSocket` protocol, described in the specification RFC 6455, provides a way to exchange data between the browser and the server via a persistent connection. The data can be passed in both directions as “packets” without breaking the connection or needing additional HTTP requests.

WebSocket is especially great for services that require continuous data exchange, e.g. real-time trading systems and so on.

## A simple example
To open a WebSocket connection, we need to create `new WebSocket` using the special protocol `ws` or `wss` in the url. Here is how you can do that in `JavaScript`:

```
let socket = new WebSocket('wss://ws.derivws.com/websockets/v3?app_id=1089');
```
