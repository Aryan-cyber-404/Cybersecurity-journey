#### log investigation 

### Do :-
    -> Run:
        journalctl -n 40
    -> Then:
        journalctl | grep sudo
    -> Observe:
        privilege usage
        warnings
        failures
    -> Question:
        -> Why do logs matter more than assumptions?
            -> logs shows the records of logins to the system
            -> It reveals timestamp , events , user and current directory 
            -> Also shows users their code execution or process execution with details 
            -> it matters because it helps us detect unauthorized access or attacks 
            -> if there happens to be any suspicious activity it helps investigate .