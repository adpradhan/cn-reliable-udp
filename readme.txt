NSUU Protocol 

***Group Members***

Rupsa Dhar - 2018A7PS0376H
Rishabh Jain - 2018A7PS0275H
Pranavi Marripudi - 2018A7PS0507H
Adesh Kumar Pradhan - 2017B3A70960H
Mereddy Aishwwarya Reddi - 2018A7PS0276H

***How to run***

Open two terminals.

    -On one terminal, type the command >>python3 server.py
    -On another termincal, type the command >>python3 client.py

These two are the server and client terminals respectively. 
The client will be prompted to enter a filename that it wants from the server. The file will be saved as 
client_<filename>.<extension> once the transfer is successful.

***Libraries used***

socket
threading
time
hashlib
base64
sys
os

***Phase-2 Protocol Modifications***
The following changes were made to NSUU protocol from phase-1

1. Size of an UDP packet (MSS) has no restriction and carries 1024Bytes of file data
2. Ack timeout is changed to 0.5secs from 1sec
3. Maximum retransmission is reset to 300
4. Cumulative Ack concept has been introduced
5. After successful transfer of file, server sends Fin Data Packet to Client for it to terminate