lib for sockets
 - communication protocol!!! like (smtp , https, http , ws)
 - 



- brodcaste ka matlab -> jo join krega usko nhi dekega ki voh join kra hai !!1
		- baki sab ko pta chlega ki voh join kra hai


<span style="color:rgb(0, 176, 80)">io        → global broadcaster<br>socket    → single client connection<br><br>socket.on   ← receive<br>socket.emit ← send to self<br>io.emit     ← send to all<br>broadcast   ← send to everyone except sender<br></span> 


io.on("connection", (socket) => { ... })   // new client
io.emit("msg", "sabko bhejo")              // all clients
io.to("room1").emit("msg", "room ko")      // room