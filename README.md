# Websocket Go

### Running Locally

run the following command to start the server:

```bash
go run main.go
```

### Testing

To test, open the webdev tools in multiple tabs, the console and run:

```javascript

//creates a connection to the WS
let socket = new WebSocket("ws://localhost:3000")

//handles receiving messages from the server
socket.onmessage = event => console.log("from server: ", event.data)

//send a message to be broadcasted 
socket.send("message")
```
