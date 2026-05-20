### Process investigation

## Linux runs many processes 

So today i wanted to see :-

-> I typed "ps" in my linux terminal. I noticed some section like user and PID etc...
-> Then i typed "ps aux "
    i saw many sections which are :-
        USER
        PID
        %CPU
        %MEM
        VSZ
        RSS
        TTY
        STAT
        START
        TIME
        COMMAND

-> Then i observed 
    procss id(PID) which are assigned in ascending order
    Process name which are the commands actually running
    user which shows me who runs command or which host controls the command 
    memory usage shows me the memory it takes to run a ccommand

-> After that i typed "top"
    then i observed that "top" is a command name . and that line is highlighted..
    it basically identifies the highest cpu and memory usage of individual command

# Q. WHy would cybersecurity analysts care about running processes ?
-> To detect malware or malicious program 
-> To detect unauthorized access (hackers)
-> Find persistence mechanisms (hackers often keep access after compromising a machine) *reverseshell attack
-> Investigate high CPU and meomry usage  *cryptojacking
-> Spot suspicious parent-child relationship
-> Incident response and forensics

So,basically Cybersecurity analysts monitor running processes to detect malware, suspicious behaviour,unauthorized access ,resource abuse and signs of compromise..

