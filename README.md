# Real-Time-Video-transfer
creating a connection between client and server using TCP sockets and to   demonstrate real time video transfer.  Implemented using Python (OpenCV).

For demonstrating Video transfer using Python create two files in python one is for the client-side and the other is for the server-side. Now use the stream socket where the server code with extracting the video from the server webcam and then it will send that video to the client using socket programming.

I have created a socket with two parameters. The first parameter is AF_INET and the second one is SOCK_STREAM. AF_INET refers to the address-family ipv4 and SOCK_STREAM means connection-oriented TCP protocol.

The server will create the socket and will go to the listening mode. Initially, the server will not require the IP address of the client 

Information is sent and received using send() and recv() function. Here we will use TCP as a streaming protocol which means there are no message boundaries it is just the stream of message bytes. 

At the client-side first, we will unpack the received packet data using struct module and then will load the frame using pickle, and finally, we will display the received video.

At the client-side first, unpack the received packet data using struct module and then load the frame using pickle, and finally, and display the received video.
