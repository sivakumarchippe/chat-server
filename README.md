# chat-server
How to Run the Chat Server

1. You need to specify the port number when running the server program from the command line. For example:

``java ChatServer 8989``

- This starts the server listening on the port number 8989, and you see the following output in the server once it started:

``Chat Server is listening on port 8989``

- The server is waiting for new clients forever, so you have to press Ctrl + C to terminate it.

2. How to Run a Chat Client
   To run the client, you need to specify the server’s hostname/IP address and port number in the command line. For example:

``java ChatClient localhost 8989``

- This tells the client to connect to the server at localhost on port 8989. Then you see the following message in the server’s console:

``New user connected``

- And in the client’s console:

``Connected to chat server``

``No other users connected``

- You see, the server tells the client how many users are connected, but there’s no user at this time. Then the program asks for the username:

``Enter your name:_``

- Enter a username, say csk, and then you can start chatting:

``Enter your name: csk``

``[csk]:_``

- Now, let’s start the second client with username is msk. At this time, you see the server tells that there’s one online user is csk:

``Connected users: [csk]``

- The user csk is notified about new user msk:

``New user connected: msk``

- Type some messages from csk and msk and you see each user sees other’s messages, just like talking in a chat room.
  Now, csk wants to quit so he types ‘bye’- the client program terminates, and you see the following output in the server’s console:

``The user csk quitted``

- msk also gets a message from the server:

``csk has quitted.``