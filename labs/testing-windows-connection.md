---
cover: >-
  https://images.unsplash.com/photo-1523961131990-5ea7c61b2107?crop=entropy&cs=srgb&fm=jpg&ixid=MnwxOTcwMjR8MHwxfHNlYXJjaHw2fHx0ZWNofGVufDB8fHx8MTY0ODQ0MDAzMQ&ixlib=rb-1.2.1&q=85
coverY: 0
---

# Testing Windows Connection

1.

{% embed url="https://youtu.be/vBwvuf5D01M" %}

In this video, we'll be testing our connection from our Windows machine and our threat emulation host.

1. On your threat emulation host, open up the terminal.  If a window pops up with "Untrusted application launcher", choose the "Mark Executable" option.
2. Start the Caldera server.  `cd caldera/` , `ls` to make sure you are in the right directory, and start the server with the following command `python3 server.py --insecure`
   1. This may take a moment to start up. By default, Caldera is enabled on port 8888. When you see the "All systems ready" log, you should be ready to log in.&#x20;
3. We're going to test to see if the login works now. Using Remina Remote Desktop, we are going to use the "Quick Connect" feature to login to our Windows workstation. Once connected, login using the appropriate credentials.

This is the preferred method to be able to complete the subsequent labs. This allows you to easily copy and paste between machines.&#x20;
