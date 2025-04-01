
# Cybersecurity Incident Report (Server TCP Attack)

| **Section 1: Identify the type of attack that may have caused this**  **network interruption** | |
| --- | --- |
| One potential explanation for the website's connection timeout error message since it is being experienced by multiple people and not one person which would rule out host slow internet connection would be website server issues. Upon reviewing the TCP logs in Wireshark we have found that there are increased SYN requests from I.P. 203.0.113.0 that increase in frequency before the RES, ACK is performed by the server stating that it is under too much load and resetting to which this does not alleviate the issue. This event is clearly an SYN Flood DOS attack due to the attack coming from only one IP address. | |
|

| **Section 2: Explain how the attack is causing the website to malfunction** |
| --- |
| When website visitors try to establish a connection with the web server, a three-way handshake occurs using the TCP protocol:   1. SYN = Synchronize : Device requests to initiate connection with server   2. SYN/ACK = Synchronize / Acknowledge : Server received the packet and acknowledges that it has received the packet from the initial computer.  3. ACK = Acknowledge : Connection is officially established with the server  When an attacker floods a server with ACK requests that are too much for the specific server then it becomes overloaded and slowed down to the point of resetting itself or completely crashing if there's not any protocols in place for protection against DOS attacks. The logs have indicated that the server is under a SYN Flood DOS attack due to the flooding of SYN packets and only on I.P. Address being the one flooding the server. This affects the server by exhausting resources, overloading the queue, and denying service to all parties. |

**Wireshark Logs**

![](data:image/png;base64...)![](data:image/png;base64...)![](data:image/png;base64...)![](data:image/png;base64...)![](data:image/png;base64...)![](data:image/png;base64...)![](data:image/png;base64...)

