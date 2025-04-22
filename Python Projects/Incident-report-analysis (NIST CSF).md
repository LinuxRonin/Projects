

**Incident report analysis**

**Instructions**

As you continue through this course, you may use this template to record your findings after completing an activity or to take notes on what you've learned about a specific tool or concept. You can also use this chart as a way to practice applying the NIST framework to different situations you encounter.

| **Summary** | This evening our network & its services became unusable for around two hours. Our security team ended up discovering that we were under a DDOS attack. The attackers were able to shut down out network for hours and flood the server with ICMP packet pings because of a completely unconfigured firewall. |
| --- | --- |
| Identify | Our company’s cybersecurity team audited the systems, networks and servers that came under attack and found that the threat actor gained unauthorized access to our network via unsecured firewalls. |
| Protect | **The team is therefore implementing new firewall policies and filters for both incoming and outgoing traffic to control the rate of ICMP packets, installing network monitoring software also known as SIEM tools, and installing a IDS/IPS system to filter out suspicious traffic to prevent another mishap.** |
| Detect | To detect new attacks in the future we are installing an IDS/IPS system into our network behind the firewall so that there are significantly less false positives and more protection to our clients. |
| Respond | The cybersecurity team after concluding our quick investigation shut down the network fully to prevent more damage, implemented new firewall rules, installed more deep routed security measures, and attributed resources to SIEM monitoring of our networks. |
| Recover | The team will for now on monitor our networks, periodically update and tweak as needed our networking security protocols & rules, and demand verification so that we can trace the source of all ICMP packets to its true destination and host. |

| Reflections/Notes: |
| --- |

# SCENARIO

![Text

Description automatically generated](data:image/png;base64...)

