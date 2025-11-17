# URL
https://tryhackme.com/room/whatisnetworking
# Category
Fundamentals
# Concept
Learn about networking and how devices are connected
# Method of Solve
## Task 1 
* Network is a group of devices connected toguether
* Answer is `Network`
## Task 2
* The Internet is made up of many small networks all joined together.  These small networks are called private networks, where networks connecting these small networks are called public networks -- or the Internet
* Answer is `Tim Berners-Lee`
## Task 3
* An IP address is a set of numbers that are divided into four octets. The value of each octet will summarise to be the IP address of the device on the network. This number is calculated through a technique known as IP addressing & subnetting
* A public address is used to identify the device on the Internet, whereas a private address is used to identify a device amongst other devices
* Devices on a network will all have a physical network interface, which is a microchip board found on the device's motherboard. This network interface is assigned a unique address at the factory it was built at, called a MAC (Media Access Control ) address. The MAC address is a twelve-character hexadecimal number (a base sixteen numbering system used in computing to represent numbers) split into two's and separated by a colon. These colons are considered separators. For example, a4:c3:f0:85:ac:2d. The first six characters represent the company that made the network interface, and the last six is a unique number
* Spoof the mac adress using the interface. The answer is `THM{YOU_GOT_ON_TRYHACKME}`
## Task 4
* Learn about the ping command
* What protocol does ping use? Answer is `ICMP`
* Use the interface to ping `8.8.8.8` (Google) and get the flag `THM{I_PINGED_THE_SERVER}`. The comand to ping is `ping -c 4 8.8.8.8`
