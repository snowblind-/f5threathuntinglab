Beaconing is a term used to describe a continuous cadence of communication between two systems. In the context of malware, beaconing is when malware periodically calls out to the attacker's Command & Control (C2) server to get further instructions on tasks to perform on the victim machine. The frequency at which the malware checks in and the methods used for the communications are configured by the attacker. Some of the common protocols used for C2 are HTTP/S, DNS, SSH, and SMTP, as well as common cloud services like Google, Twitter, Dropbox, etc. Using common protocols and services for C2 allows adversaries to masquerade as normal network traffic and hence evade firewalls. SSLOrchestrator provides visibility in to C2  encrypted traffic to masquerade as normal HTTP/S traffic.

While on the surface beaconing can appear similar to normal network traffic, it has some unique traits with respect to timing and packet size, which can be modeled using standard statistical and signal processing techniques. Find the encrypted message the C2 server is responding to the client.

------------------ Your mission is to identify the payload message from the C2 server ------------------

### HINT: The flag is in the server payload and is within the message body response from the server.
