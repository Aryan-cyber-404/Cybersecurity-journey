### Servic Investigation :-

Services = Programs running in background

### Commands used:-
    -> systemctl list-units --type=service
    -> systemctl status ssh
    -> systemctl status NetworkManager
    -> 

### Observations ;-
    -> Found UNITS(service names), running state (which are currently active and running), loaded service (existing services) after running first command .
    -> Found about ssh, whether it is active or not , whether it exists or not and the docs .
    -> Found aboutNetworkManager , whether it is active or not, whether it exist or not , Invocation ,docs , main PID ,tasks,memory, cpu and cgroup ...
       Herr it is active currently running.


### Q. Why do cybersecurity analysts care about services ?
-> Services reveal attack surface
-> Malware often installs itself as a service
-> Failed services can signal compromise or misconfiguration
-> Services tell you what the system is supposed to be doing 
-> Services help detect lateral movement
-> Services create logs
-> Security tools themselves are services
-> At the end, Services tell analysts where software is running. what's broken, what's exposed, and what may be malicious.

### things i learn :
-> Attackers sometimes disable logging to hide activity
-> xmrig.service = crypto miner 
-> ufw.service = firewall
-> service generates telemetry 
