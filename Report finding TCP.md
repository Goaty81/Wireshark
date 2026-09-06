<ins>TCP in Wireshark</ins>

In this document we will see how the TCP handshake is shown in Wireshark!

<img width="1140" height="119" alt="image" src="https://github.com/user-attachments/assets/51f990dd-a949-4f3f-be6e-324baea5ce01" />

Here we have the packets that we will be looking at, As you can already see the SYN handshake and the FIN handshake already in the information to the right but lets look at it more in depth!

<ins>SYN Handshake</ins>

Objective

Identify and analyse the TCP SYN three-way handshake within the packet capture(PCAP).

Filter: TCP

Evidence:

<img width="1060" height="658" alt="image" src="https://github.com/user-attachments/assets/0f56c84e-ea39-4b97-a820-1623145a6a9e" />

<img width="1135" height="670" alt="image" src="https://github.com/user-attachments/assets/6dbf1fde-aff5-41ea-b3b5-b923bd3763c9" />

<img width="966" height="697" alt="image" src="https://github.com/user-attachments/assets/3b7606a1-a230-4ae1-91db-e5e022285436" />

Analysis:

Packets 267, 289 and 291 show the SYN TCP handshake in Wireshark.

SYN — The client initiates a TCP connection.
SYN/ACK — The server acknowledges the request and indicates that it is ready to establish the connection.
ACK — The client acknowledges the server's response.

The connection is therefore successfully established.

Conclusion:

The captured traffic demonstrates a successful TCP connection establishment using the standard three-way handshake.

<ins>FIN TCP Handshake</ins>


Objective

Identify and analyse the TCP FIN three-way handshake within the packet capture.

Filter: TCP

Evidence:

<img width="990" height="650" alt="image" src="https://github.com/user-attachments/assets/48ada535-fd94-4195-bf72-8d6efe64b649" />

<img width="996" height="669" alt="image" src="https://github.com/user-attachments/assets/a07e5bdc-8b21-4137-a98a-fd65e45eefb9" />

<img width="965" height="671" alt="image" src="https://github.com/user-attachments/assets/fa5a16c8-f3c5-499a-a86b-6dcab1fa9c4f" />

Analysis:

Packets 380, 384 and 385 show the FIN TCP handshake in Wireshark.

FIN — The client initiates a TCP connection.
FIN/ACK — The server acknowledges the request and indicates that it is ready to terminate the connection.
ACK — The client acknowledges the server's response.

The connection is therefore successfully terminated.
