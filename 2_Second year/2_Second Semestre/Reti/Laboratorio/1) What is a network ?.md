In the first part of the program we define two protagonist in the connection:

1. ==Sender==
2. ==Receiver==
   
These two are now **==nodes==** (or hosts) of the network !
So...Now i'll describe the phases of connection:

1. The ==sender== sends a message to the ==receiver==  through a signal
2. The signal passes through the cable or wi-fi (these are called ==medium==)
3. But the messages must follow a set of rules for the transmission that are included in ==protocols== ! 
   
   NB: the message can be a ==request== or a ==resource ==
   
   
-------------------------------------------------------
1.1 What are nodes / hosts ?

Host are divided into ==clients== and ==serves==
A host could behave both as a client and a server.

![[Pasted image 20260428235233.png]]

As we can see in this image the ==client== sends a ==message request== to the ==web Server== but...

The web Server could also behave as a client when for example he needs information such as credential of the client / user

NB.  The server also are computer BUT they've software which is able to respond

As we know the computers have multiple network ports, so we could connect with a cable the computers with each other. But as the number of devices increases, the complexity of the topology increases as well. For these reason and others we can use a ==Hub== or better a switch

-------------------------------------------------------
1.2 What is a Hub ?

A Hub is a network device that allow us to connect multiples computers. But isn't smart cause hubs simply sends messages to all the ports without searching the hostRequest

![[Pasted image 20260429153106.png]]

-------------------------------------------------------

1.3 Bridge

The ==bridge== is another network device can resolve the problem of sends message to all the ports cause it can be ==learn== which host is connected of one his two network ports.  

![[Pasted image 20260429154112.png]]

------------------------------------

1.4 Switch

The ==switch== finally is an combination of an hub and a bridge ! 

Cause it can be connected multiple host just like an hub 

And it can learn / recognize the combination host / network port

And these two factors allow this network device to ==send the response== at the correct host and with this network device ==we've finally got a good network==

![[Pasted image 20260429155423.png]]  

Network in fact is a graph how multiple nodes / hosts are connected to which others and for this reason they can sends and receives messages in the correct path and and most important only the correct host can receive

![[Pasted image 20260429160222.png]]

--------------------------------------


1.5 router

Connect networks is the role of ==router==:
The router can:

1. Connect different network
2. Act as a ==gateway== for the node (when a host knows that a message isn't in the local network he send the message to the router...and for this reason he acts as a gateway for the host ! cause allow the public interface) 
   
Also the router can be connected to each other ! in fact we can say that internet is a network of interconnected router !

But now...Exercise time !!


------------------------------------

The assignment:

Try to design a network topology as follow:
  

- There are a Home Network
    
- There are 5 devices connected to the network
    
- The Home Network is connected to the City Network
    
- In the City Network there are other 2 Home Network
    
- Via a Gateway, the City Network is connected to the Internet
    
- At some point, a YouTube Network is connected to the Internet
    
- Inside the YouTube Network, there are 2 nodes, the Video Streaming Server and the Database Server.








NOTATION:
1. The IP address is compose by 32 bit (4 * 8)![[rete1.excalidraw]]

2. If the last is "0" he's identify the network
   `192.168.1.0` 
   
3. if the last is "255" he's identify all hosts 