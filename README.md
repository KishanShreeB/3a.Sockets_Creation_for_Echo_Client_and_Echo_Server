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
 ## NAME:KISHAN SHREE B
 ## REG NO:212223100022
## PROGRAM
~~~
## CLIENT 
import socket
s=socket.socket()
s.connect(('localhost',8000))
while True:
  msg=input("Client > ")
  s.send(msg.encode())
  print("Server > ",s.recv(1024).decode())

## SERVER
import socket
s=socket.socket()
s.bind(('localhost',8000))
s.listen(5)
c,addr=s.accept()
while True:
  ClientMessage=c.recv(1024).decode()
  c.send(ClientMessage.encode())
~~~

## OUPUT
![image](https://github.com/user-attachments/assets/b79669d8-fde0-44d8-ba94-85cba71d43d8)
![image](https://github.com/user-attachments/assets/8114d1b8-5bc5-4bdf-b55d-161f74b13814)


## RESULT
Thus, the python program for creating Echo Client and Echo Server using TCP Sockets Links 
was successfully created and executed.
