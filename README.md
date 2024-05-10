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
## PROGRAM
```
Client:
Divya P
212223040044

import socket
s=socket.socket()
s.connect(('localhost',8000))
while True:
 msg=input("Client > ")
 s.send(msg.encode())
 print("Server > ",s.recv(1024).decode())

Server:
import socket
s=socket.socket()
s.bind(('localhost',8000))
s.listen(5)
c,addr=s.accept()
while True:
 ClientMessage=c.recv(1024).decode()
 c.send(ClientMessage.encode())

```
## OUTPUT:

![WhatsApp Image 2024-05-10 at 13 35 05_68254cb5](https://github.com/DivyaP0110/3a.Sockets_Creation_for_Echo_Client_and_Echo_Server/assets/144870891/de5b92f9-ab36-4212-ac49-f467cdd01212)

![WhatsApp Image 2024-05-10 at 13 35 12_12ad1d1b](https://github.com/DivyaP0110/3a.Sockets_Creation_for_Echo_Client_and_Echo_Server/assets/144870891/9b562cfd-9f4b-4474-b860-1e3a931e8b43)


## RESULT

Thus, the python program for creating Echo Client and Echo Server using TCP Sockets Links was successfully created and executed.
Thus, the python program for creating Echo Client and Echo Server using TCP Sockets Links 
was successfully created and executed.
