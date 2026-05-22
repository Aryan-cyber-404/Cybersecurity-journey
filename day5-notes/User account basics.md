#### User-accounts basics :-

### Commands used:- 
    -> cat /etc/passwd 
    -> cat /etc/passwd | grep bash

### Observations :-
    -> i found so many lines like this : "root:x:0:0:root:/root:/bin/bash" 
        where root : username
        x : paassword placeholder
        0: UID
        0: GID
        /root : home folder
        /bin/bash : login shell 

    -> i found only lines with word "bash" . And this is important because users with bash shell are usually real login-capable users. 

### Q. Why might attackers care about user accounts? 

    User accounts are important to attackers because :
    -> it can give access to the attackers 
    -> attackers can modify , delete or install harmful files 
    -> they can also access sudo and take full control of the system by cracking week passwords .

    so, basically user acoounts are front doors of the system . 
    