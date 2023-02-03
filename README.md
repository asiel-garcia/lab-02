# Lab 2
[Fork](https://docs.github.com/en/get-started/quickstart/fork-a-repo) this repo and clone it to your machine to get started!

## Team Members
- team member 1
- team member 2

## Lab Question Answers

Answer for Question 1: 
When the 50% loss was added to the UDP, the reliability decreased by a very noticible amount. This occurred because UDP is an unreliable transport method that does not contain error detection and therefore the delivery of packets is not guaratneed.

Answer for Question2:
The reliability of the TCP has stayed the same, it was very reliable. This is because it has error detection and so it checks if anything sent was also recieved, not limited to packets.

Answer for Question 3:
The speed of the TCP decreased with the added loss. This is most likely because it is much more complex and also has to recheck to make sure all of the transmitted data was recieved while UDP does not.
...

Code Questions:

Q1) argc is the argument count, so it will be the total number of arguments in the command line when running a file. *argv[] is the argument vector that is and array of pointers to arrays of character objets which basically points to all the string inputs in the command line.

Q2) A UNIX file descriptor is a number that identifies and open file in the computer's OS and is unique. A file descriptor table is the collection of integer array indicies that are file descriptors in which elements are pointers to file table entries. It translates the file descriptor in the table to an open file.

Q3) A struct is a data type that defines a physically defined group of variables under one name in a specific block of memory. The sockaddr_in is used to store address for the internet address family. It is used to define a socket address.

Q4) The input parameters of socket() are (int domain, int type, int protocol).
domain- specifies the communications domain in which a socket is to be created
type- specifies the type of socket
protocol- specifies the specific protocol to be used (0 uses a default unspecified protocol)
A successful return value will be a non-negative integer which is the socket file descriptor. a value of -1 will indicate an error.

Q5) int bind(int socket, struct sockaddr *address, int address_len)
int listen(int socket, int backlog)

Q6) The use of while(1) allows the newsockfd to run completely and to only work on one accept call because if there are multiple accept calls it will result in an error if their identities are changed.

Q7) fork() is used to create a child process that runs simultaneously with the process that makes the fork() call. It can be applied with an if loop so that anytime there is a new client trying to connect to the server a new child process can be created that can run simultaneously with the other processess so that one server can attend multiple clients using TCP.

Q8) A system call is when the program calls for a service from the operating system which is then executed.
