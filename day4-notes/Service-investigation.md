### Services found :-
    ->  I found total 174 services. first i used the command "systemctl list-units --type=service -all" , then counted all of them using " systemct list-units    --type=service -all | wc -l"

### Suspicious Services:-
    ->  No i didn't find any suspicious activity or any attack surfaces in my system.

### Running state :-
    ->  then i used the command "systemctl list-units --type=service state=running" , it tells me all the running service at the moment ..

### Logs Observed :-
    -> i observed the failed , exited, dead, running states of sevices in the system.

### Open ports :-
    -> I didn't find any open ports .

### Security thoughts :-
    -> I should investigate throtoghly if there is any unnecessary open ports ..
    -> also try to solve the case if have to ...

I did this project from perspective of a junior analyst .....