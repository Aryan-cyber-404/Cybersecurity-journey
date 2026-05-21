### Privilege Basics 

### Commands used:-
    -> whoami
    -> id
    -> sudo -l

### Observetions:-
    -> found my user
    -> found uid , pid , gid ,group 
    -> Matches different entries for user


### Q. Difference between normal user and root user 

    ## Normal user:-
        -> Limited permissions
        -> can use regular apps and files
        -> cannot install/change system files without permissions
        -> Safe for daily use
    
    ## Root user :-
        -> Full control odf system
        -> Can change anything
        -> Can install , delete, modify everything
        -> powerful but risky

### Q. Why is giving unnecessary sudo access risky ?

    ->  Sudo is like a master key of the system . it can take full control of the system .
    -> if any outsiders enter the system by chance with unnecessary sudo access they can take control of the full system .
    -> They can delete , modify ,stel data/files easily 
    -> least privilege = give only the access someone actually needs .
    