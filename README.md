# CS_570_HW5
==================
Build Instructions
==================

To build the program, run "make" within assignment root directory.  Makefile includes RPC gen command.

==================
Usage Instructions
==================
To run the server program, run "./server". 

***
To run the client program, run "./client hostname", where hostname is the name of the host running the server, e.g., "./client localhost" if the server is running on the same host.
***

The client program has the following functions available: 

Open: Requires a filename. Opens the file with the given name. If file doesn't exist for loggedin user, create one. Returns file descriptor (fd) for open file, and -1 if error occurs.
Read: Requires file descriptor, number of bytes to be read, and pointer to a buffer where content should be stored. Returns as content char of '0' if any error occurs.
Write: Requires file descriptor, number of bytes to be written, and pointer to a buffer where content to be written is stored. Returns a message describing result of the operation.
List: Returns a list of all files owned by logged in user
Delete: Requires a filename. Deletes file with the given name owned by user.
Close: Requires a file descriptor. 