#### Port investigation :- 

### Commands used:- 
    -> ss -tulnp
    -> nmap localhost

### Observations :-
    -> I found port number ,tcp/udp protocols , State(listen,disable) and process 

    Then i choose one port 
    -> i choose port 123 .
    -> i tried to find about this port using "sudo ss -tulnp | grep 123" 
    -> i found its pid , gid and its service name. hre pid is 987
    -> i typed "ps -p 987 -f" to find its processes
    -> i typed "systemctl status ntpd(service name i found)" 
    -> it gave the full details about it. 
    -> i found that it is network time protocol daemon . it synchronizes time of the system with network time . 

    Then i used nmap localhost to see what's the differnce :
    I found:
    -> nmap scans addresses , and here it is local host which is 127.0.0.1
    -> this tool is used to check networking stack of the system , also used for debugging 
    While,
    -> ss tool scans ports to check activity of ports . checks state of ports , if there is any open ports then it helps to investigate about that service. 

### Q. Why is an unnecessary open port risky ? 
-> open port which shows "LISTEN" state in the system. It means it is waiting for communication in that port. WHich produce attack surface.
-> if there is any unnecessary open ports or outdated service. Then it is easier for attackers to commnicate with this port . so there shouldn't be any open ports with no reason.
-> Also a cybersecurity analyst first investigates the open ports . he/she investigates timestamp , process name , logs , cpu usage and service names . If there is any suspiciousness then doing deep investigation ceases the attack.
