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


Analysis

Packets 1–3 demonstrate the TCP three-way handshake.

SYN — The client initiates a TCP connection.
SYN/ACK — The server acknowledges the request and indicates that it is ready to establish the connection.
ACK — The client acknowledges the server's response.

The connection is therefore successfully established.

Screenshot




Conclusion

The captured traffic demonstrates a successful TCP connection establishment using the standard three-way handshake.
