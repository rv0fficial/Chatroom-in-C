# Chatroom-in-C

A simple Chatroom built in C programming language. The program has two files - <b>server.c</b> and <b>client.c</b>. The program is built uses multithreading for handling multiple clients.

## Run Locally

### Compile the Server:
Open a terminal and navigate to the directory containing the server file (`server.c`). Run the following command:

```bash
gcc -pthread -o srv server.c
```

This command compiles the server code and generates an executable named `srv`.

### Run the Server:
 Execute the compiled server program by running:
```bash
./srv
```

This command starts the server, and it will begin listening for incoming connections on the default IP address "127.0.0.1" and port 66666.

### Compile the Client:
Open another terminal and navigate to the directory containing the client file (`client.c`). Run the following command:
```bash
gcc -pthread -o cli client.c
```

This command compiles the client code and generates an executable named `cli`.

### Run the Client:
Execute the compiled client program by running:
```bash
./cli 66666
```

This command starts the client and connects it to the server running on IP address "127.0.0.1" and port 66666. Adjust the port number if you want to use a different one.

### Repeat for Additional Clients:

Open new terminals and run additional instances of the client to simulate multiple clients connecting to the server.

```bash
./cli 66666
```
Note: Make sure to run the server first before starting any clients. Also, ensure that the IP address and port specified in the client code match the server's IP address and port. 
