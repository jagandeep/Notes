# Notes

Book: Web Scalability for Startup Engineers

Chapter 7 : Asynchronous Programming

Synchronous programming : Caller calls and wait for the call to complete
Asynchronous programming: Caller calls and doesn't block and continues execution
and it notified later through callback or API to get the result.

Blocking : means waiting for operation to finish.
Blocking can be CPU or I/O
CPU means waiting for compuation to finish
I/O means waiting for reading from the database, file system, network or user inpput are all example of i/o.


Message Queue
- A way to archive asynchronous/non blocking processing in application designed for synchnronous programming 
- decouples producer and consumer which allowes them to scale indepenently.
- coupled only on the address of queue and message format.

Message Broker
 message queue can be implmented in many ways 
 - a simple thread running in same application.
 - shared folder were application read and write to 
 - compnenet implemented on SQL database
 - an application accepting, routing, persisting and delivering message( few others as well permission control, failure recovery) aka Message Broker or MOM or EMS.

 They are optimised for 
 - high concrrency 
 - high throuput 
 - fast message enque
 

