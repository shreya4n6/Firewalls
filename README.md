# Firewalls :fire:

## FIREWALL :

:sun_with_face: It is a device that monitors and controls incoming and outgoing traffics based on some predefined rules<br>
:sun_with_face: It acts like a barrier <br>

 ## HOST BASED AND NETWORK BASED FIREWALL:

Host based is the one which we have predefined in our personal computer systems. In other words it is a software based firewall.
In Network based firewalls, there is a dedicated hardware on which the firewall software runs.

For ex: our private company is the internal (trusted) network . The network outside the private company is untrusted or external(public) network. Here, comes the role of firewall in between these two. How will the company know that from where the traffic is coming from. It can be malicious or any attack can be performed. Hence, firewall blocks the malicious ones and allows only the right traffic to flow as per its rules.

## NOW WHAT ARE DATA PACKETS ?

When we want to download a file say 200MB from the internet. We wont receive the entire 200MB data at once. But we will receive small packets, say 5MB every second. Some part of the 5MB data contains information about the sender , receiver and IP address and the rest part contains the actual data which we are downloading. Hence, part of the actual data + the information together form data or IP packets. This part of the actual data is referred to as the payload. 

## TYPES OF FIREWALL:

### :anger: PACKET FILTERING FIREWALL: 
It checks IP header and TCP header attached to the downloaded file. In other words it will check the IP address and port number. 
Works on network and transport layers.
IP address or even the full network can be blocked
Can block a service (http,ftp etc)

The rules of Access Control List are used for data packet verification. If everything is okay it is allowed to pass through the firewall and then to my laptop. Packet Filtering Firewalls are present in internet routers and its less secure. Its limitation is the it does not check the payload or the data packet. A hacker can send malicious data here.

### :anger: APPLICATION/PROXY FIREWALL :

Proxy firewall does not let the internet know which laptop wants the requested website. It hides us from attackers on the internet. It hides the IP address of the sender and forwards the request to the internet. It also checks the payload but it is slower than packet filtering firewalls.When the user client process sends a message, the proxy firewall runs a server process to receive the request. The server opens the packet at the application level and confirms whether the request is legitimate or not. If it is, the server acts as a client process and sends the message to the real server, otherwise the message is dropped. In this way, the requests of the external users are filtered based on the contents at the application layer

### :anger: HYBRID FIREWALL :

It combines the application firewall and packet filtering firewall in series. It provides the best security as compared to the other two firewalls. It protects user’s servers and workstations from malicious problems and unauthorized access.


INTRUSION DETECTION SYSTEM(IDS) AND INTRUSION PREVENTION SYSTEM(IPS)

IDS and IPS both work together in order to detect intruder activity on our network and once intruder activity is found, appropriate steps are taken in order to stop the activity. So IDS and IPS can either be a hardware or combination of hardware and software which we can deploy on our network and web app in order to detect intruder activity. 

### :fireworks: INTRUSION DETECTION SYSTEM

It's basically a passive system that scans incoming traffic. Once the IDS identified dangerous or suspicious traffic it sends alerts but sends the action to IPS

This is a system which can detect the threats, malware and unauthorized activity over the network and also monitor the suspicious activity and intimate the network administrator for action.
This is a monitoring and detection system or tool.
It does not take action on their own. The network administrator takes the action detected by IDS

## There are four types of IDS:

:umbrella: Network Intrusion Detection System (NIDS)<br>
:umbrella: Host Based Intrusion Detection System (HBID)<br>
:umbrella: Perimeter Intrusion Detection System (PIDS)<br>
:umbrella: VM based Intrusion System<br>

### :fireworks: INTRUSION PREVENTION SYSTEM

This is a system which can prevent or protect the system or network from threats, virus and suspicious activities and can take action against these activities. 
It is a control system or tool
It takes the action automatically i.e, accepts or rejects packets based on the rule set. It is like a firewall.

To see the default firewall rules setup from you terminal using:

### Iptables -L 




