<ins> Report findings - DNS</ins>

In this document i will be reporting my DNS findings on Wireshark!

The Image below is a image from Wireshark of 3 Conversations from the Client Host to the DNS server querying about the Domain name of a Server Host.

<img width="1580" height="121" alt="image" src="https://github.com/user-attachments/assets/c4c520d4-a212-40c8-865f-0d9f77f68afc" />

I will be using this template for all findings:

Filter: 

Relevant packet:

Observation:

Screenshot 1:

Screenshot 2:

Ports:

Conclusion:

As you can see they are all different and i will go into them in more depth right now!

<ins>HTTPS</ins>

Filter: DNS

Relevant packet: Packet numbers 1097, 1102

Observation: The Client Host has sent a HTTPS query about the Server Host to the DNS server, The DNS server has responded with a HTTPS response.

Screenshot 1: <img width="963" height="289" alt="image" src="https://github.com/user-attachments/assets/1054fc1b-c43f-4bac-97b8-9b15db1c79fc" />

Screenshot 2: <img width="1004" height="301" alt="image" src="https://github.com/user-attachments/assets/9688d814-77dd-408a-b376-1f99968262c2" />

Ports: 49665, 53

Conclusion: The Client Host has sent a HTTPS query of the Server host to the DNS server through a IPv4 connection and ports 49665 and 53 (consisting of 592 bits). The DNS server has then sent a response back to the Client Host about the HTTPS query and has verified that it has a HTTPS Domain name for the Server Host (consisting of 1584 bits).

You may also see that the answer is "Unsolicited:True", This could mean that it hasn’t matched another query to this packet although it knows the Client Host sent one or this could be signs of a security flaw.

Security flaws associated with this are:

  - DNS Cache Poisoning/ Spoofing
  - DDoS attack

<ins>IPV4</ins>

Filter: DNS

Relevant packet: Packet numbers 1099, 1100

Observation: The Client Host has sent a query about the Server Host to the DNS server.

Screenshot 1:<img width="970" height="284" alt="image" src="https://github.com/user-attachments/assets/eec89bb5-7126-4fd7-936d-cd67eabebe41" />

Screenshot 2:<img width="962" height="300" alt="image" src="https://github.com/user-attachments/assets/ae137a22-16ae-4f35-bea2-af5097a84126" />

Ports: 50291 (unassigned port), 53 (DNS)

Conclusion: This time instead of a HTTPS query it is a IPv4 query, The Client Host has sent a query to see if the DNS server has a domain connection with the Server host through IPv4, The DNS server has responded with another "true" answer. This signifies that there is a IPv4 connection!

<ins>IPv6</ins>

Filter: DNS

Relevant packet: Packet numbers 1099, 1100

Observation: The Client Host has sent a query about the Server Host to the DNS server.

Screenshot 1:

Screenshot 2:

Ports: 50291 (unassigned port), 53 (DNS)

Conclusion:
