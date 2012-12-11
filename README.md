To compile just run make from command line.

To compile this code you will need gcc and make.

debian: apt-get install build-essential
centos: yum install make && yum install gcc


you@server:/folder/path/# make

To use run
you@server:/folder/path/# ./annoying_server portnumber &

use jobs to see what servers you are running

to test the server use telnet to the port number

telnet 127.0.0.1 portnumber

example: 

./annoying_server 21 &
[1] 13682

you@server:/folder/path# telnet 127.0.0.1 21
Trying 127.0.0.1...
Connected to 127.0.0.1.
Escape character is '^]'.
what is it
Here is the message: what is it

I got your messageConnection closed by foreign host.

YAH! You now have an annoying server to setup during ctf.

Use make clean to delete and binary so you can recompile

you@server:/folder/path# make clean


