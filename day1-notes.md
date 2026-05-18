# Day 1 notes 

### commands learned :-

#### pwd
Prints or Shows current directory

#### ls
List information abot files 

#### cd 
Change directory 

#### mkdir 
Create a directory , if they do not exist 

#### cp
Copy files and directories 

#### mv
Rename files 

#### rm
Remove files/directories

#### cat
Concatenate files to standard output

#### clear
Clear the terminal screen

#### history
It's a GNU history library where logs , lines associated with data were recorded

#### whoami 
Print the user name or current user-id

#### uname -a
Print all the information abot certain system


### System information investigation :-

#### ip a 
Shows or manipulates routing ,network devices ,interfaces and tunnels .
If we want to know our ip address , simply we have to run thi command "ip addr" . it shows ip addresses assigned to all network interfaces .

#### ifcongig
It is basically used to configure network interfaces .
used at boot time to setup interfaces .

#### ping google.com
Ping basically used to send requests to network hosts and requests come under ICMP(Internet Cintrol Message protocol) .
Here i have written "ping google.com" . It means i am sending requests to network host named "Google.com"

#### netstat -tulnp
netstat prints information about linux networking subsystem.
here -tulnp is the bucket of -t , -u, -l, -n, -p 
and -t shows TCP connections
-u shows UDP connections
-l shows only listening sockets 
-n displays addresses and port numbers numerically
-p shows the PID and name of program using socket 
So, "netstat -tulnp" lists all listening TCP and UDP ports, shows the process ID /PID and uses numeric addresses and ports .

#### ss -tulnp 
ss used to dump socket statistics . it shows informations like netstat but it can display more inormation about TCP and UDP state than other tools..

#### Q1. How Can i find my ip address ?
I will type "ip addr show" or "ip a" in terminal . Then it shows interfaces of IPv4 and IPv6 addresses. 
e.g.:- inet 127.0.0.1/8 
it indicates an IPv4 address of 127.0.0.1 with 8-bit subnet mask

#### Q2. What is loopback address ?
It is a virtual interface used for interal communication , it always have the IPv4 address 127.0.0.1/8 and IPv6 address ::1/128 ..
it allows servics to communicate with the locall system without using physical hardware.
it is basically comes under "lo" section where it is written loopback,up,lower up when typing "ip addr" or "ip a " command in terminal.

#### Q3. How can an user identify the state of interface ?
AN interface is ctive(UP) if it can send/receive files..
to know this type " ip link show up" in terminal 
state up indicates an active interface while state DOWN means inactive

#### Q4. What are listening ports ?
When we findout the information about information of linux subsystem 
there it shows some TCP/UDP ids in listening state those are the listening ports.


### Networking Theory :- 

#### OSI model -
it consists of total seven layers ,which are:
Application layer - interfaces directly with end-user applications [LEVEL 7]
Presentation layer - Translates, encrypts, and compresses data for secure and efficient transmission [LEVEL 6]
Session layer - Establishes, manages and terminates communication sessions between devices [LEVEL 5]
Transport layer - Ensures reliable data delivery, flow control, error checking and segmentations [LEVEL 4]
Network layer - handles logical addresses and routing of data betwyyn networks [LEVEL 3]
Data link layer - Organizes datainto frames,handles MAC addessing , and error detection on local networks [LEVEL 2]
Physical layer - Tranmits raw bitstreams over physical media [LEVEL 1]

#### TCP/IP model - 
The apllication layer,transport layer, network layer and data-link layer of OSI model comes under the TCP/IP model..

#### TCP Vs UDP -
TCP stands for Transmission Control Protocol . It prioritizes reliability and accuracy
UDP stands for User Datagram Protocol . It prioritizes speed and low latency

#### Ports and Protocols -
Network ports and protocols define how data is transmitted and received over a network .
Ports act as communication end points numbered from 0 to 65535 while protocols determine ruleers for data exchange 

Protocol     Port
HTTP         80
HTTPS        443
SSH          22
DNS          53
FTP          21
SMTP         25 

### Reconnaissance :-

#### Open port - 
basically take window as a door and computer as a house .. like an open door waiting to receive data from computer,server or database etc..
e.g.:-
PORT      STATE    SERVICE 
80/tcp    open      http
5432/tcp  open      postgresql 

#### sevice detection :-
findig out the exact name and version number of the program behind open door 

#### Why attackers scan first ??
 to see which door is open and what programs are running so that they can find weekness 
