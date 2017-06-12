# ELK-NXLog-Config
Files required on Server and Clients to install ELK Stack for NXLog Windows Event collection




Instructions for configuring WEF and nxlog/ELK:




1. Configure WEF server and clients 
-there are plenty of tutorials on this and it's fairly straightforward
--e.g. https://blogs.technet.microsoft.com/jepayne/2015/11/23/monitoring-what-matters-windows-event-forwarding-for-everyone-even-if-you-already-have-a-siem/
--https://docs.microsoft.com/en-us/windows/threat-protection/use-windows-event-forwarding-to-assist-in-instrusion-detection
-you will be done once your systems are forwarding specified logs to a collector




2. Configure an ELK system to receive events
-use the following tutorial exactly 
--make sure you use Ubuntu 14.04 and follow instructions provided
-https://www.devopslibrary.com/lessons/elk-stack-for-logging-tutorial

2a. Reconfigure ELK system for specific events from WEF system
-use elasticsearch.yml, kibana.yml, and logstash.conf files in this repo
--MAKE SURE TO SWAP THE SERVER IP WITH YOUR ELK SERVER IP ADDRESS





3. Configure WEF collector system to send ForwardedEvents to ELK system
-use the nxlog.conf file in this repo
--MAKE SURE TO SWAP THE SERVER IP WITH YOUR ELK SERVER IP ADDRESS
