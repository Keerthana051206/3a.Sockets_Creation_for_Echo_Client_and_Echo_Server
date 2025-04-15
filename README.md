# 3a.CREATION FOR ECHO CLIENT AND ECHO SERVER USING TCP SOCKETS
# AIM
To write a python program for creating Echo Client and Echo Server using TCP
Sockets Links.
## ALGORITHM:
1. Import the necessary modules in python
2. Create a socket connection to using the socket module.
3. Send message to the client and receive the message from the client using the Socket module in
 server .
4. Send and receive the message using the send function in socket.
5. PROGRAM:
6.
## PROGRAM
```
 clint
  import socket
s=socket.socket()
s.connect(('localhost',8000))
while True:
msg=input("Client > ")
s.send(msg.encode())
print("Server > ",s.recv(1024).decode())
 server
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
client
<img width="277" alt="image" src="https://github.com/user-attachments/assets/6363bcf2-a7dd-489b-8560-7bb99c667816" />

 server
 <img width="273" alt="image" src="https://github.com/user-attachments/assets/604d76d2-f7fe-4543-9a18-11b499cfb3c0" />


## RESULT
Thus, the python program for creating Echo Client and Echo Server using TCP Sockets Links 
was successfully created and executed.
