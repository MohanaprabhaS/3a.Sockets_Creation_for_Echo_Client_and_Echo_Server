# 3a.CREATION FOR ECHO CLIENT AND ECHO SERVER USING TCP SOCKETS
# NAME: MOHANAPRBAHA S
# REGISTER NO: 212224040197
# DATE:15.5.25
# AIM
To write a python program for creating Echo Client and Echo Server using TCP
Sockets Links.
## ALGORITHM:
1. Import the necessary modules in python
2. Create a socket connection to using the socket module.
3. Send message to the client and receive the message from the client using the Socket module in
 server .
4. Send and receive the message using the send function in socket.
## PROGRAM
```
Client

import socket 
s=socket.socket() 
s.connect(('localhost',8000)) 
while True: 
msg=input("Client > ") 
s.send(msg.encode()) 
print("Server > ",s.recv(1024).decode())

Server

import socket 
s=socket.socket() 
s.bind(('localhost',8000)) 
s.listen(5) 
c,addr=s.accept() 
while True: 
ClientMessage=c.recv(1024).decode() 
c.send(ClientMessage.encode())
```
## OUPUT

![Screenshot 2025-05-12 162306](https://github.com/user-attachments/assets/226aa100-362d-4ae5-b4b1-02cf3fa87570)


## RESULT
Thus, the python program for creating Echo Client and Echo Server using TCP Sockets Links 
was successfully created and executed.
