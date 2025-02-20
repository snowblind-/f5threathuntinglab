# Security Onion – First Time User’s Guide
Security Onion is a free and open platform built by defenders for defenders. It includes network visibility, host visibility, intrusion detection honeypots, log management, and case management. For network visibility, it offer’s signature based detection via Suricata, rich protocol metadata and file extraction using either Zeek or Suricata, full packet capture using either Stenographer or Suricata, and file analysis.

The Security Onion Console can be reached from within the lab by browsing to https://10.1.1.8. Login using the provided credentials. 
![alt text](/Images/SO_login.jpg "SO Login")

After logging in, you will see the Security Onion Console (SOC) Overview page:
![alt text](/Images/SOC_overview.jpeg "SO Overview")

From here, you can navigate to Dashboards by clicking the Dashboards link on the left-hand side of Security Onion Console. The Dashboards page provides an overview of all logs and alerts. 
![alt text](/Images/SO-Dashboard.jpeg "SO Dashboard")

From within the Dashboard page, you can filter event datasets by left mouse-clicking on an event data of interest, then clicking the appropriate filter button.
![alt text](/Images/SO_dashboard_filter.jpg "SO Dashboard Filter")

To focus on alerts only, you can navigate to the Alerts page by clicking the Alerts link on the left-hand side of the page.
![alt text](/Images/SO_alerts.jpeg "SO Alerts")

To see the individual events associated with an alert, you can left-click one, then click the Drilldown button. This will filter the display to only those events associated with the alert.
![alt text](/Images/SO_event_drilldown.png "SO Drilldown")

If you see something interesting from either the Dashboards or Alerts screen, you can quickly pivot to the Hunt screen by left-clicking the Alert or Event, expanding the Actions dropdown, then clicking the Hunt button.
![alt text](/Images/SO_event_hunt.png "SO Event Hunt")

This will take you to the Hunt page. From here you can search and filter through events.
![alt text](/Images/SO_hunt.jpeg "SO Hunt")

Also from within the Hunt page, you can either create custom queries(beyond the scope of this document), or use one of several predefined queries by clicking the dropdown in the top left portion of the query bar.
![alt text](/Images/SO_query_dropdown.png "SO Query Dropdown")

If you find interesting network traffic, you can pivot to full packet capture via the PCAP action. This is found from within the same action menu as Drilldown and Hunt. From within this screen, you can change the view to an ASCII transcript OR send the pcap to CyberChef.
![alt text](/Images/SO_pcap.jpeg "SO PCAP Action")

PCAP ASCII Transcript
![alt text](/Images/SO_pcap_details.jpeg "SO PCAP Details")

PCAP details in CyberChef. CyberChef can also be used to encode/de-encode data using the operations actions on the left-hand side of this screen.
![alt text](/Images/SO_cyberchef.jpeg "SO CyberChef")

Finally, the below is a simplified example workflow using Security Onion:
- Go to the Alerts page and review any unacknowledged alerts.
- Review Dashboards for anything that looks suspicious.
- Once you’ve found something that you want to investigate, you might want to pivot to Hunt to expand your search and look for additional logs relating to the source and destination IP addresses.
- If any of those alerts or logs look interesting, you might want to pivot to PCAP to review the full packet capture for the entire stream.
- Depending on what you see in the stream, you might want to send it to CyberChef for further analysis and decoding.




