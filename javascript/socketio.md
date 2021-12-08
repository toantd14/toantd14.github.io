# PART: SOCKET.IO

## QUESTION

1.  


## REFERENCE
- [Socket.IO](https://socket.io/)
- [BeeChat App Sample](https://github.com/mytechlabo/node-chat-app-realtime)

## KEY NOTE

1. Key Note
- Connect, Disconnect, Reconnect
  - `^socket.on()` : *client listen event*
  - `^io.on()` : *server listen event*
- Message
  - `^socket.emit()` : *client push message to server or server push message to client*
  - 
  - `^socket.broadcast.to(^room).emit()` : *server push message to client in room (has connect before)*
  - `^io.sockets.in(^room).emit()` : *server push message to client in room*
  - `^io.to(^room).emit()` : *server push message to client in room*
  - 
  - `^socket.broadcast.emit()` : *server push message to all client connect socket (has connect before)*
  - `^io.sockets.emit()` : *server push message to all client connect socket*
- Ping, Join and Leave
  - `^socket.join(^room)` : *join current user to room*
  - `^socket.leave(^room)` : *leave current user from room*
- Namespaces
  - `^io.of(^namespace)` : *logging namespace of socket io*

### Help
1. `^socket`: *variable*
2. `^io`: *variable*
3. `^room`: *room name (list user id)*
4. `^namespace` : *space name*


