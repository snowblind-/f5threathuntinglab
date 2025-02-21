In this Capture the Flag (CTF) challenge, participants will investigate a data exfiltration scenario where a malicious attacker is attempting to covertly transfer sensitive data outside the network. The challenge focuses on network visibility and threat detection using F5 SSL Orchestrator, which provides decryption and inspection capabilities to analyze encrypted traffic.

Scenario:
A company's sensitive customer records have been compromised, and security analysts suspect an employee or attacker is exfiltrating data using encrypted channels. However, traditional security tools fail to detect the anomaly due to encrypted traffic. Participants must use F5 SSL Orchestrator to decrypt, inspect, and analyze network traffic to identify the exfiltration method, malicious endpoint, and attacker’s tactics.

Objectives:
Decrypt and analyze traffic using F5 SSL Orchestrator.
Identify the protocols and techniques used for data exfiltration.
Trace the attacker’s actions and determine the destination of exfiltrated data.
Extract the flag hidden in the exfiltrated data or network logs.

Skills Required:
Network traffic analysis (PCAP analysis)
Understanding of TLS/SSL decryption and F5 SSL Orchestrator
Identifying covert exfiltration channels (DNS tunneling, HTTP/S, FTP, etc.)
Threat hunting and forensic investigation.

This CTF is designed to enhance participants' incident response, threat detection, and network security skills while demonstrating the importance of SSL decryption for deep packet inspection in modern cybersecurity environments.

Your mission is to find the node that is transmitting this data and its endpoint. You need to find the payload being transferred.  Inside the payload is the CTF flag.

Good Luck!
