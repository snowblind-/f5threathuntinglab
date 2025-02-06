# Challenge Number.1 - DNS Beaconing

DNS beaconing is a technique often used in cybersecurity, primarily by attackers, to communicate with compromised devices or systems. It involves sending DNS (Domain Name System) requests that are designed to transmit small pieces of data, or "beacons," to an attacker’s server, often in a covert or hidden manner.

In DNS beaconing, the compromised system sends out DNS queries that appear normal, but the information being sent within these queries can contain exfiltrated data or serve as a way for the attacker to track the infected system. These requests are typically sent to a domain that is controlled by the attacker.

The key features of DNS beaconing include:

Covert Communication: DNS is widely used for normal internet operations, so it can be difficult to detect beaconing activity. Attackers take advantage of this to evade detection from security systems that might not monitor DNS traffic as closely as other types of network traffic.

Exfiltration or Command and Control: The beaconing can either send out information from the compromised system (exfiltration of data) or request instructions (commands) from the attacker’s server.

Periodicity: The compromised system often sends DNS requests on a regular interval, which can make it easier for the attacker to maintain communication with the system without raising suspicion.

Size and Structure of DNS Requests: The attacker may encode data into the DNS request, often using the subdomain part of the DNS query to carry the exfiltrated data.

It's an advanced method of maintaining persistence in a network, often used in sophisticated attacks like APTs (Advanced Persistent Threats), since it blends in with normal internet traffic. Detecting DNS beaconing often requires looking at unusual patterns of DNS queries, like high volumes, odd domain names, or unexpected frequency.
