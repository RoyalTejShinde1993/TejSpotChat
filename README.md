# TejSpotChat
TejSpot-Networking-Project, C++ ,  The communication between the Server and Client based on TCP  The communication between two Clients based on UDP
# Networking-Programming-Project , TejSpotChat , C++

The final project is a hybrid P2P and client­server messenger application
that enable two clients to send and receive messages between one and the
other

The developed project implement the following functionality:

* The project include two apps: Messenger Server App (MSA) and
 Messenger Client App (MCA).
* The communication between the MCA and MSA based on TCP 
(control messages).
* The communication between two MCA’s based on UDP 
(interaction between two clients).
* Messenger Server App and Messenger Client App using a CLI
* Programming in C++ in eclipse (JavaEE) / Linux enviroment

Guidelines:

## Messenger Server App CLI:
* lu - list all users</br>
* lcu - list all connected users</br>
* ls - list all sessions (two clients communicating)</br>
* lr - list all rooms</br>
* lru <room name> - list all users in this room</br>
* x - shutdown</br>

## Messenger Client App CLI:
* c <IP> - connect to the server in the given ip</br>
* lu - print the user list from the server</br>
* lcu - print the connected users list</br>
* lr - print all rooms</br>
* lru <room name> - print all users in this room</br>
* login <user> <password> - login with the user and password</br>
* register <user> <password> - register the new user with the given password and login the user.</br>
* o <username> - open a session with the user</br>
* or <room name> - enter a chat room user can be connected to only to one other user or chat room at a
time, calling o or or commands will disconnect other open session.</br>
* s <message> - send a message</br>
* l - print the current status of the client (connected to “xyz”/not connected) </br>
* cs - disconnect the open session / exit from a room</br>
* cr <room name> - close a room</br>
* d - disconnect from server</br>
* x - close the app</br>


### To connect to the server the client will sign in using a username and a password (no encryption required):
* The client can create a new user with a new password (unless this user is already created).</br>
* To communicate with another client, the user will request to open a session with the required user name.</br>
* The list of usernames and passwords will be saved into a file in the server side.</br>

### Chat rooms (conference chat):
* The client is able to open a chat room.</br>
* A chat room may be closed only by its creator.</br>
* Each client can enter a chat room or leave it.</br>
* Once a client enters a chat room it will receive all messages sent by all the other clients in the room, and all the clients will
receive his messages.</br>
* In order not to overload the server, all client communication is
P2P using UDP and does not pass through the server.</br>

