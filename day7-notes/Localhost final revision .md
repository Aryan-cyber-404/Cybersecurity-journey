#### Localhost final revision 

### Do :- 
    -> Question:
        -> Difference between:
            127.0.0.1 and 192.168.x.x
    -> Answer :
        -> # 127.0.0.1 :
            -> it is loopback address of the user 
            -> It is also local address of an user on surface 
            -> it runs without netwotk connectivity.
            -> analysts most prefer this address because of security and protection
            -> any user connected to lan can't access this network .
            -> it is also used for debugging and checking networking-stack
            -> basically this address doesn't travel outside
        -> # 192.168.x.x :
            -> It is address of a device over the network 
            -> analyst use this type of address to scan the network
            -> every other devices has different ip addresses unlike localhost address 
            -> It needs network connectivity for execution
            -> This address travells outside carrying data traffic 