# Application used :- 
Wireshark

# commands in terminal :-
    ping 127.0.0.1
    ping google.com

# filter usedin wireshark:-
    ICMP

# Q. Difference between localhost traffic and internet traffic in wireshark 

1. ping 127.0.0.1:- 

-> Traffic stays inside the computer because 127.0.0.1 is local loopback address.
-> packets do not go the router or internet.
-> After filtering icmp there is no result . but for icmp6 there are some results.

2. ping google.com :-

-> Traffic goes outside of computerthrough the internet.
-> DNS request happens first to resolve 'google.com' into an ip address.
-> ICMP packets travel over the internet to google's server.
