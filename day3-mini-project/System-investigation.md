#### System investigation report - Day3 

#### Objective 
The objeective of this investigation was to observe system processes, open ports, logs, and networking behaviour to better understand how linux system operates.

### System process :-

## Commands used :-
-> ps 
-> ps aux
-> pstree

## Observations :-
-> multiple running processees
-> found system services running in background
-> noticed cpu and memory usage 

## security relevance:-
-> identify suspicious process
-> detect malware
-> investigate resource abuse
-> find unathorized applications 

### Open ports and services:- 

## Commands used :-
-> ss -tulnp
-> netstat -tulnp 

## Observations :-
-> Found listening ports
-> Observed local services running
-> Identified networking-related services 

## Security Relevance :-
-> Open ports increase attack surface 
-> Unnecessary open ports may :
    |- expose vulnerable service
    |- allow un authorized access
    |- reveal information about system software 

### Log investigation :-

## Commands used :-
-> journalctl -n 20 

## Observaations :-
-> Observer timestamps
-> Found system events
-> Saw service-related logs

## Security Relevance :-
-> Logs help analysts:
    1. investigation incidents
    2. identify suspicious activity
    3. troubleshoot problems
    4. detect failed logins 

### Networking Investigstion :-

## Commands used:-
-> ping 127.0.0.1
-> ping google.com

## Observations:-
-> Localhost(127.0.0.1) : Traffic stayed inside the machine
-> Google ping : Traffic traveled exernally and ivolved internet communication
-> So, Localhost is used for internal testing while external communication uses network connectivity. 

#### This mini project i built for one reason .That is to stay focused as cyber-analyst and making report upon incident
