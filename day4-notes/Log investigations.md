### Log investigaton (deeper):-

### Commands used :- 
    -> journalctl -n 30
    -> journalctl --since today 
    -> journal ctl --since today | grep "failed"
    -> journalctl | grep sudo

### Observations :- 
    -> Found Service events with timestamps and found some failed activities and warning  in 30 statements
    -> Then found same informations as above since the system i started. it gave ame all log records
    -> Then found the failed activities using grep search method.
    -> Found the logs about sudo . also found the commands i used using sudo .

### Q. Why are failed login attempts important ? 
 ->  If there is one or two failed login attempts , user might have forgotten the password
 -> But if there is too many failed login attempts , then there is someone trying to break in..
 