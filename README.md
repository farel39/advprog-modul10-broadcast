# Module 10 - Broadcast Chat

## Sending message from clients
![Sending message from clients](./send_msg.png)

### How to run it
#### * Running the Server
```bash
cargo run --bin server
```

The server will start listening on port 2000. You should see a message indicating it's "Listening on port 2000".

#### * Running Clients
In separate terminal windows, run multiple clients:
```bash
cargo run --bin client
```
You can run as many clients as needed to participate in the chat.

### What happens when i type some text in the clients.

When you type a message in any client:
1. The message is sent to the server
2. The server receives the message and broadcasts it to all connected clients
Every client (including the sender) displays the message prefixed with "From server:"
