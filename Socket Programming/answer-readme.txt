(2) Try running the program immediately again when it finishes
    successfully. What do you see? Why? What happens when you remove the various
    sleep()s in the program?

This is what we get originally without any change to the code:
[S]: Server socket created
[S]: Server host name is ilab4.cs.rutgers.edu
[S]: Server IP address is 128.6.4.28
[C]: Client socket created
[S]: Got a connection request from a client at ('128.6.4.28', 51484)
[C]: Data received from server: Welcome to CS 352!

This is what happens after remove sleep()s:
[S]: Server socket created
[C]: Client socket created
[S]: Server host name is ilab4.cs.rutgers.edu
[S]: Server IP address is 128.6.4.28
[S]: Got a connection request from a client at ('128.6.4.28', 52040)
[C]: Data received from server: Welcome to CS 352!

So, after remving sleep()s, we can notice that the sequence of building connection between server and client has changed. "Client socket created" step is now two steps before get server host name and IP address.


