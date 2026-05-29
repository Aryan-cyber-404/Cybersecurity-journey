### Revision practical

### Do 1:-
    -> Run:
        -> whoami
        -> id
        -> groups
    -> Question:
        What powers does your user have?
    -> Answer: 
        User have access to system files , photos , videos ,documents etc.
        Can own their home directory
        Can run programs
        Can create processes and network connections.

### Do 2 :-
    -> Run:
        ->ss -tulnp
    -> Pick one port
    -> Question:
        -> Why is this port open ?
        -> Needed or unnecessary ?
        -> What risk exists ?
    -> Answer:
        I will take an example of port 22 (SSH service)
        -> port 22 is open it means it is waiting for communication. and here SSH service is waiting for communication . if it is not intentional or being required then it is risky
        -> It is needed because if there is unnecessary ssh service is open and if any attacker has already on the line to commnicate with it then it can lead to major issue .So if there is any activity like this , as a analyst the first step to take is to investigate .
        -> Risks:
            -> Brute force and password attacks
            -> Credential stuffing
            -> Explotation of SSH vulnerabilities
            -> privilege escaltion 
            -> Full sever takeover
            -> Information disclosure

### D0 3 :- 
    -> Run:
        -> ps aux --sort=-%cpu | head
    -> Question:
        -> What would make a process suspicious?
    -> Answer :
        -> when a process has high cpu usage , it is suspicious .
        -> when there is command or service name includes /tmp .. it is suspicious .
        -> when there is unusual name .... it is suspicious .