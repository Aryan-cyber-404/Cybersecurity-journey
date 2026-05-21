### Service management 

### Commands used :-
    -> systemctl status bluetooth
    -> sudo systemctl stop bluetooth
    -> sudo systemctl start bluetooth

### Observations :-
    -> Found bluetooth service is not active but it exists in the system
    -> Then i tried to stop that function and saw that there is no change 
    -> then i restart the bluetooth service.

### Q.Why might attakcers create hidden services ?
-> Attackers create service which restart automatically and this is called persistence(service reboots) .
-> Blend in legitmate service through masquereading (pretending to be something legitmate) .
-> remote access / command and control 
-> Avoid detection because many security tools focus on processes or user actions.
-> Services sometimes run with elevated permissions , if attackers can install or modify one , they can gain powerful access.
-> Disable defenses through stop logging , weaken monitoring , tamper witjh firewall behaviour 
-> Especially against companies , attackers want to stay hidden for weeks or months. The quiter they are , they stay longer unnoticed 

-> Every service should have a reason to exist .