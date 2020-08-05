# Echo Websocket Server using Tornado Framework(python)

This is an implementation of a simple websocket server on localhost. It echoes back whatever data is sent to it to all its connected clients.

1. On connecting to localhost:8888/ the server sends a webpage to client.
1. Upon recieving the webpage the client automatically gets connected to the websocket server at localhost:8888/ws
1. On successful connection client recieves a confirmatory message.
1. Then a state is sent by the server(introduced from pespective of multiplayer games, current state can be sent to newly connected client).
1. Message sent from any client to the server is echoed to all the clients connected to the server.


### Prerequistes-
* Tornado python package. Install for python3 on Ubuntu using-
```
pip3 install tornado
```

Tornado is a web app framework specifically designed to handle asynchronous operations. See official documentation at-

https://www.tornadoweb.org/en/stable/

### Setting up server- 
* Clone the repository.
* Navigate inside the repo and type the following in the terminal -
```
python3 server.py
```
Your server is up and running on localhost:8888.

### Connecting to the server-
* Open your web-browser and in the url bar type the following and hit enter-
```
localhost:8888/
```
* Messages can ne sent/recieved through this web page to/from the server.



### Acknowledgements - 
* Major help from amazing article on basics of tornado framework and asynchronous programming at -
https://opensource.com/article/18/6/tornado-framework

* Took inspiration from Ramesh Sampath's implementation of Tic-Tac-Toe game using websockets-
https://github.com/sampathweb/board-games-app
