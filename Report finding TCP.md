<ins>TCP in Wireshark</ins>

In this document we will see how the TCP handshake is shown in Wireshark!

<img width="1140" height="119" alt="image" src="https://github.com/user-attachments/assets/51f990dd-a949-4f3f-be6e-324baea5ce01" />

Here we have the packets that we will be looking at, As you can already see the SYN handshake and the FIN handshake already in the information to the right but lets look at it more in depth!

<ins>SYN Handshake</ins>

Objective

Identify and analyse the TCP SYN three-way handshake within the packet capture(PCAP).

Filter: TCP
Evidence:

<img width="1057" height="765" alt="image" src="https://github.com/user-attachments/assets/d1fe274a-966c-4abc-8b02-1e9ea86bc829" />

<img width="1132" height="770" alt="image" src="https://github.com/user-attachments/assets/5a057f38-9e1d-4722-8fe1-5228544cee60" />



Analysis

Packets 1–3 demonstrate the TCP three-way handshake.

SYN — The client initiates a TCP connection.
SYN/ACK — The server acknowledges the request and indicates that it is ready to establish the connection.
ACK — The client acknowledges the server's response.

The connection is therefore successfully established.

Screenshot




Conclusion

The captured traffic demonstrates a successful TCP connection establishment using the standard three-way handshake.
