---
layout: page
title: "royalscape"
date: 2016-03-14 23:33
comments: true
sharing: true
footer: true
---
![alt text](http://i.imgur.com/Na7omyk.jpg "Players")
![alt text](http://i.imgur.com/rRKQxFo.jpg "Server")

Introduction
---------------------

Royalscape is an emulation of the popular MMORPG Runescape.
A server was developped over a period of four years with a goal of emulating the real Runescape servers. 
The client was obtained via reverse engineering and the server was written in Java. Though a small project, the emulated server was able to attract around 70 players daily and stable enough to make multiplyer playable at reasonable frame rates. 

Technology
---------------------
Deobfucation of the original Runescape client was required in order to obtain a working game client to be used in compliance to the server. 
Client wise, the majority of the work was in learning exactly how the client should communicate with the server and vice versa. The tricky part was identifying what packets were being sent out and which should be sent in. Since the packet recieving and sending code were all obfucated it was difficult to unwind and understand what each packet's indended use was. 

The server sided development of this project was more laborious because everything had to be emulated to a certain degree of accuracy so that the game was playable. Networking was handled by NIO. After player interactions and networking details, the addition of new content was enjoyable because it allowed for deviation and customization that was limited by Runescape's actual servers.