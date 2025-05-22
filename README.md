# Tutorial 10 - Broadcast

## FIRST COMMIT 

### 1. ![img](/img/image1.png)
</br>
The four terminal windows illustrate a successful multi-client chat application using TCP sockets in Rust. In the top-left window, the server is started with cargo run --bin server, listening on port 2000. As three clients connect (from the other three terminals), the server logs their connections and receives their messages: “halo saya ilham”, “halo saya fam”, and “halo saya delf”. Each client, started with cargo run --bin client, displays a welcome message and sends one message input by the user. The server broadcasts each received message to all connected clients, including the sender. This is evident as every message appears in all three client windows regardless of which one originally sent it. The real-time message relay confirms that the server correctly handles concurrent client connections and broadcasting functionality, forming a basic but functional chatroom system.</br>



## SECOND COMMIT

### 1. ![img](/img/image2.png)
In the screenshot, the server is running and listening on port 2000, as indicated by the message "listening on port 2000." However, the client is configured to connect to port 8080 instead. Since no service is listening on port 8080, the client's connection attempt is refused by the operating system. This results in an I/O error with code 10061 and the message "No connection could be made because the target machine actively refused it." The client process then terminates with a failure exit code. This mismatch between the client’s target port and the server’s listening port is the cause of the connection failure.

### 2. ![img](/img/image3.png)
However, after i change the port on server.rs, everything went back to normal.

