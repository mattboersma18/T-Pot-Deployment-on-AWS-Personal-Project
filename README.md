# T-Pot-Deployment-on-AWS-Personal-Project
This project is designed to deploy a T-Pot honeypot on an AWS ubuntu server. The goal of this project is to see real world data and attacks in real time.

For this project, I used a personal Ubuntu Server, as well as an Amazon AWS Instance in order to deploy my Honeypot.
I started first with deploying the AWS EC2 Instance, this instance would allow me to keep my home devices safe from any potential issues that may arise. We make sure that in order to access the server we setup a key file, so that the instance can only be accessed from machines with that Key. Creating an extra layer of security for the Ubuntu Server. To start, the only port that should be open is the Home port to access the server.

Once we are inside our AWS instance, we can install our honey pot using https://github.com/telekom-security/tpotce, this honeypot is an open source platform that we will use to collect attakcs. Once installed we can now change our AWS instance to accept multiple different port numbers to subject our honey pot to outside traffic. Allowing certain ports of different types to access the honeypot is what we will use to collect actual data.

Now that we can access our Honeypot menu, we can see the different types of data
![This is the general display where out data is being collected](honeypotScreenshot1.png)

This T-Pot honeypot dashboard (Kibana, October 10-12, 2026) recorded roughly 3,000 attacks across six honeypots. Tanner, the web application honeypot, was hit most (about 1,000), followed by Cowrie (SSH/Telnet, 694), RDPHoneypot (475), H0neytr4p (471), Dionaea (460), and Ciscoasa (1). The most targeted ports were 80, 3389, 443, 445, and 23, showing that web, remote access, and file-sharing services draw the most attention. Traffic was low and steady for most of the period, with large bursts on October 11-12 that point to automated scanning or botnet activity. Attacks came from around the world, led by the United States, India, Egypt, Hong Kong, and South Korea, and most source IPs were flagged as web attackers, mass scanners, or otherwise having a bad reputation. Attacker systems were mostly Linux, with some Windows, likely compromised servers or IoT devices. Overall, exposed services are probed constantly, and most of this activity appears opportunistic and automated.

![This is the bottom half of the display that displays more data](honeypotScreenshot2.png)
Like the top half of the data, the bottom half shows us some interesting information. 