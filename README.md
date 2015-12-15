# ODR-Protocol
Development of a client/server application where the messages are exchanged using an ODR protocol

Authors: Gagan Nagaraju (109889036) & Harishkumar Katagal(109915793)
CSE 533 - Assignment 3
********************************************************************************************

• An On Demand shortest hop Routing Protocol (ODR) for routing messages in networks of fixed but arbitrary and unknown connectivity was implemented using PF_PACKET sockets.
• A client/server application was developed in which the messages were exchanged using ODR.
• An API that enables applications to communicate with the ODR mechanism was developed using Unix domain datagram sockets.

#USER DOCUMENTATION:

Following are the files that contain the source codes for the assignment 3.
client_hkatagal.c
server_hkatagal.c
get_hw_addrs.c
hw_addrs.h
odr_hkatagal.c
odr_hkatagal.h
utilities.c
utilities.h



To compile and generate executables use the "Makefile" and issue a "make". This will generate the *.o and the executable files. The three main important files that we want are "server_hkatagal", "client_hkatagal" and "odr_hkatagal". Use these three files to run the server, client and odr respectively. To run the server use "./server_hkatagal" command, this will starts the server and creates listening sockets. To run the client use "./client_hkatagal". To run the odr use "./odr_hkatagal 10". Specify the staleness parameter as argument to run this program.
Some sample examples are shown below.

Ex1:   	./server_hkatagal
		./client_hkatagal
	   
Note: When you issue make, you might get some warnings like "warning: assignment from incompatible pointer type", these can be safely ignored.

Output:
All the messages from the server, client and odr are displayed in their corresponding terminals.

**************************************************************************************************
