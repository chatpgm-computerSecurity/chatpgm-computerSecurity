
# Chat Application

This project is a simple client-server chat application that allows multiple clients to communicate with each other. The server listens for client connections and relays messages to all connected clients except the sender.
## Group Members - 
1) DEVIKA SALIMKUMAR
2) KRISHNA REVANTH KURUMETI
3) AASISH SAJJA

## Features
- Server handles multiple clients simultaneously using threads.
- Clients can send messages and receive messages from other connected clients.
- Server distributes messages to all connected clients.
- Simple text-based communication between clients over a TCP connection.

## Components

1. **Server**: Listens for client connections and facilitates communication between multiple clients.
2. **Client**: Connects to the server and allows users to send and receive messages.
3. **Client 2**: A second instance of the client to demonstrate multiple clients communicating through the server.

## Prerequisites

- **Windows OS** (uses `WinSock2` for networking)
- **Visual Studio IDE** with C++ support (no external compiler required)

## How to Run in Visual Studio

### 1. Clone the Repository
```bash
git clone https://github.com/chatpgm-computerSecurity/chatpgm-computerSecurity.git
cd chat-application
```

### 2. Open the Project in Visual Studio
- Launch **Visual Studio**.
- Select **File > Open > Project/Solution**.
- Navigate to the folder where you cloned the repository
- Open the `.sln` solution file (if available) or add the `.cpp` files manually for server, client, and client2 folders seperately in each windows of Visual Studio.


### 3. Build the Project
- Once the projects server, client, and client2 windows seperately.For is open, select **Build > Build Solution** (or press `Ctrl+Shift+B`).
- Ensure that the build is successful for all the three windows(server, client and client2). Any errors will be displayed in the output window.

### 4. Run the Server and Clients
- After the build is successful, press the **Run** button (`F5` or the green play button) for each component (server, client, and client 2). 
- Visual Studio will launch a command prompt for each component: one for the server and separate ones for the clients.

### 5. Communication
Once the server is running, start both clients. You will be prompted to enter your chat name. After that, you can start sending messages, which will be broadcast to all other connected clients except the sender.

To quit the chat, type `quit` and press `Enter`.

## Sample Output

### Server Output:
```
Server has started listening on port: 12345
Client connected
Client connected
Message from client: User1 : Hello
Message from client: User2 : Hi!
Client disconnected
```

### Client Output:
```
Enter your chat name:
User1
User1 : Hello
User2 : Hi!
```
### Outputs screenshots

### 1. Server starting and connecting to the client
![Server starting and connecting to the client](outputs/image1.png)

### 2. Client successfully connecting to server
![Client successfully connecting to server](outputs/image2.png)

### 3. Client messages
![Client messages](outputs/image3.png)

### 4. Client disconnecting from from server
![Client disconnecting from from server](outputs/image4.png)

## Known Issues

- If a client disconnects abruptly, the server may take time to detect the disconnection.
- Only basic text-based chat is supported. No file transfers or media sharing.

  

