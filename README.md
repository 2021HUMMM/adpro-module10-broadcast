# Tutorial 10 - Broadcast

## FIRST COMMIT 
</br>
The four terminal windows illustrate a successful multi-client chat application using TCP sockets in Rust. In the top-left window, the server is started with cargo run --bin server, listening on port 2000. As three clients connect (from the other three terminals), the server logs their connections and receives their messages: “halo saya ilham”, “halo saya fam”, and “halo saya delf”. Each client, started with cargo run --bin client, displays a welcome message and sends one message input by the user. The server broadcasts each received message to all connected clients, including the sender. This is evident as every message appears in all three client windows regardless of which one originally sent it. The real-time message relay confirms that the server correctly handles concurrent client connections and broadcasting functionality, forming a basic but functional chatroom system.</br>

