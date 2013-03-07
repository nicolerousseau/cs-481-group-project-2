cs-481-group-project-2
======================

Our project consists of two programs: MessageReader, and MessageWriter. 
MessageReader is a server program that simply prints whatever is sent to it. 
MessageWriter connects to a remote host and sends messages to it. 
Both programs can be run on the same machine using the hostname "localhost" or IP address "127.0.0.1".

In one terminal session, run:

$ java MessageReader 10001

This will start the server, which will block waiting for connections. 
Once it receives a connection, it will print whatever is sent it.

In another terminal session, run:

$ java MessageWriter localhost 10001

You will see a prompt like this:

>>> 

When you see this prompt, you can type a message to be sent. 
Press <ENTER> to send the message to the server. 
When you do, you will see the message appear in the terminal that's currently running MessageReader.

Two-way communication can be achieved by running another instance of both MessageReader and MessageWriter, 
using another port (say, 10002).
