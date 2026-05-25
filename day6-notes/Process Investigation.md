#### Process Investigation 

### Commands used :-
    -> ps aux --sort=-%cpu | head 

### Observations :- 
    -> I found user ,PID ,CPU usage ,stat and time stamp 
    -> THis command is used to check heavy usage of cpu in different commands running . 

### Q. Why would analysts care about high cpu processes ?
    -> Analysts would care about high cpu processes because 
        -> it checks the valid or invalid cpu usage like if there is a malware which uses so much of cpu . It can detect that activity.
        -> Also detect the crypto mining if it is agaist you .. 
        -> Also shows us hidden activity .