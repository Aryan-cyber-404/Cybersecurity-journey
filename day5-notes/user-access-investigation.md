### User Access Investigation Report - Day 5 

### Objective :- 
-> The purpose of this investigation was to understand :
    -> Linux User sessions
    -> login activity
    -> user accounts
    -> open ports
    -> authentication-related logs. 

### command :- 
    -> who:-
        Found currently logged-in users
    -> w:-
        Found system activity using
    -> lastlog:-
        Found login history 
    -> cat /etc/passwd :-
        Found system users and login-capable users
    -> cat /etc/passwd | grep bash:-
        Observed usernames, shells and home directories
    -> journalctl | grep failed :-
        observed failed logins
    -> journalctl | grep sudo :-
        checked sudo activity and failures 

### Investigation :- 
    -> used "ss -tulnp" and did these actions :
        ->-> port investigation
        ->-> purpose
        ->-> security thought
        ->-> Security relevance

### Wireshark Observation :- 
    -> DNS:
        -> Observed domain name resolution (google.com -> ip address)
    -> TCP:
        -> Observed communication while loading website 
    -> Learninf:
        -> DNS converts names into ip address
        -> TCP provides reliable communication

### Key Learning from Day 5:
    -> how users sessions are tracked
    -> why login history matters
    -> importance of user accounts
    -> how ports expose services
    -> why failed logins attempts matter 

### Challenges faced:-
    -> last command did not work my system so,
    -> i install login in my linux
    -> then i saw the results

### Final reflection :
    -> This investigation helped me understand how cybersecurity analusts monitor users, authentications, and system access to identify suspicious activity. 