# T-Pot-Deployment-on-AWS-Personal-Project
This project is designed to deploy a T-Pot honeypot on an AWS ubuntu server. The goal of this project is to see real world data and attacks in real time.

For this project, I used a personal Ubuntu Server, as well as an Amazon AWS Instance in order to deploy my Honeypot.
I started first with deploying the AWS EC2 Instance, this instance would allow me to keep my home devices safe from any potential issues that may arise. We make sure that in order to access the server we setup a key file, so that the instance can only be accessed from machines with that Key. Creating an extra layer of security for the Ubuntu Server. To start, the only port that should be open is the Home port to access the server.

Once we are inside our AWS instance, we can install our honey pot using https://github.com/telekom-security/tpotce, this honeypot is an open source platform that we will use to collect attakcs. Once installed we can now change our AWS instance to accept multiple different port numbers to subject our honey pot to outside traffic. Allowing certain ports of different types to access the honeypot is what we will use to collect actual data.

Now that we can access our Honeypot menu, we can see the different types of data
![This is the general display where out data is being collected]()