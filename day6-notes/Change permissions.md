#### Change Permissions 

### Objective:-
    -> experiment on security-test file ...

### Commands used :-
    -> touch security-test.txt 
    -> ls -l
    -> chmod 777 security.txt 
    -> chmod 644 security.txt 

### Observation :- 
    -> I first created a text file named security-test
    -> Then i typed "chmod 777 security.txt" on terminal after that i typed "ls -l" .. It showed the permission ehich is (read,write and execute)
    -> Then i typed "chmod 644 security.txt" on terminal after that i typed "ls -l" .. It showed me the premission of read , write then read only . 
     
### Which feels safer and why ?
    -> In this scenario i feel the permisiion of only read and write is safe which is executed by the command "chmod 644" because even if it is editable but it willl not execute 
    -> But chmod 777 is dangerous because it can be accessed , modified and executable ...