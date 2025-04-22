
# Security incident report

| **Section 1: Identify the network protocol involved in the incident** |
| --- |
| The network protocol involved in this incident is port 80 which is in control of Hypertext transfer protocol (HTTP). |
|

| **Section 2: Document the incident** |
| --- |
| We received reports from customers that they were running into a similar website of ours (yummyrecipesforme.com vs, greatrecipesforme.com) and that on this new website it was listing the recipes for free and the customers also reported that their computers started to run slower after this incident. After a deep dive into our servers and running a tcpdump on these websites we gathered enough information to see that port 80 (HTTP) was being used to perform an IP spoof attack by changing the host ports from 36086 to 56378 & as well perform a possible Man-in-the-middle attack. |

| **Section 3: Recommend one remediation for brute force attacks** |
| --- |
| Implement anti-spoofing techniques so that the IPs and ports cannot be changed as easy. |

