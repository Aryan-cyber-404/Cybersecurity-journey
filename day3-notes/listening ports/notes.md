### Listening ports

-> I typed "ss -tulnp" on terminal 

-> I observed :-
    Netid
    state
    Recv-Q
    Send-Q
    Local addresses:port
    peer addresses:port
    process

-> I saw one port which is in listening service under tcp6 protocol.

-> I tried to find ssh, browser related traffic and local services here 
    but i found nothing cause none of them are active here and i checke d through the ports
    which is SSh:22 , browser realted traffics: 80(HTTP),443(HTTPS), loal service:8080 

# Q. Why is an unnecessary open port is risky?

basically open ports gives ways to hackers to explot or hack our system. the chances of hacking increase because of open ports 
and if the ports are open with no reason, then the system will be hacked..