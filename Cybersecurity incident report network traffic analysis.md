
# Cybersecurity Incident Report: Network Traffic Analysis

![](data:image/png;base64...)

| Summary of the problem found in the DNS and ICMP traffic log. | |
| --- | --- |
| The UDP protocol reveals that Port 53 is unreachable when trying to access the site of “yummyrecipesforme.com”. This is based on the results of the network analysis, which show that the ICMP echo reply returned the error message: “udp port 53 unreachable”. The port noted in the error message is used for: Domain Name System (DNS). The most likely issue is: There are several potential issues: firewall is blocking UDP port 53, network misocnfig, DNS server is down or overloaded | |
|

| Analysis of the data and provide at least one cause of the incident. |
| --- |
| This incident occurred at 01:26 PM. We became aware of this incident after multiple reports from customers and consumers that a hosted website was down and unreachable. Our IT department loaded the website to receive the same error of destination port unreachable to which we then reloaded the page while running tcpdump to gather network information for analysis. Upon analysis using tcpdump we found that port 53 which is used by DNS is unreachable. After deep analysis of the incident we are working on several possible causes for this incident. One of them is that the firewall is blocking port 53, the other is that our network was misconfigured during an update, and lastly but most severely is that the DNS is being overloaded by a DDOS attack which will take further analysis of the logs to determine. |

