# Shared-Memory
The project was implemented as a receiver and sender program. 
The receiver program sets up a chunk of shared memory and a message queue. 
It waits till it receives a message from the sender. 
If the size of the message is not 0 then it reads the specified amount of bytes 
and saves them to a receive file and sends an acknowledgement to the sender and goes back to waiting.  
The program closes and detaches the shared memory, deallocates the shared memory and message queues, and exits 


-How to execute(from terminal):
    locationOfFiles:~$ make
    locationOfFiles:~$ ./sender keyfile.txt

from seperate terminal:
    locationOfFiles:~$ ./recv
