<ins> Report findings - DNS</ins>

In this document i will be reporting my DNS findings on Wireshark!

The Image below is a image from Wireshark of 3 Conversations from the Client Host to the DNS server querying about the Domain name of a Server Host.

<img width="1580" height="121" alt="image" src="https://github.com/user-attachments/assets/c4c520d4-a212-40c8-865f-0d9f77f68afc" />

As you can see they are all different and i will go into them in more depth right now!

<ins>HTTPS</ins>

<img width="963" height="289" alt="image" src="https://github.com/user-attachments/assets/1054fc1b-c43f-4bac-97b8-9b15db1c79fc" />

This is what a Packet looks like more closely, See that there is different drop-downs for each bit of information. However we will be using this format for each DNS finding:

Filter: DNS

Relevant packet: Packet numbers 1097, 1102

Observation: The Client Host has sent a query about the Server Host to the DNS server

Screenshot 1:

Screenshot 2: 

Ports:

Conclusion:

