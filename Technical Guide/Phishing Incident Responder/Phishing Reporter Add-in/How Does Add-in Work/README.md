# How Does Add-in Work

In Outlook where the add-in is installed, the working principle works as follows:

1. When add-in opened
	1. Sends a heartbeat to server
	2. Get order from the server, if there was an investigation or action

2. When add-in runs
	1. Sends the heartbeat to the server in periodic time¹
	2. If any order comes from the server then start to do this investigation or action²
	3. If an error occurred then it logs it to client side then send to our server

3. When outlook closes itself then add-in close


¹ The add-in optimises this process according to network and machine performance by itself.

² When conducting the investigation, the add-in optimises this process according to the computer and the network situation.