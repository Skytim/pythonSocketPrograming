# pythonSocketPrograming

    socket.socket(): Create a new socket using the given address family, socket type and protocol number.
    
    socket.bind(address): Bind the socket to address.
    
    socket.listen(backlog): Listen for connections made to the socket. The backlog argument specifies the maximum number of         queued connections and should be at least 0; the maximum value is system-dependent (usually 5), the minimum value is forced     to 0.
    socket.accept(): The return value is a pair (conn, address) where conn is a new socket object usable to send and receive        data on the connection, and address is the address bound to the socket on the other end of the connection.
    
    socket.send(bytes[, flags]): Send data to the socket. The socket must be connected to a remote socket. Returns the number of     bytes sent. Applications are responsible for checking that all data has been sent; if only some of the data was transmitted,     the application needs to attempt delivery of the remaining data.
    
    socket.colse(): Mark the socket closed. all future operations on the socket object will fail. The remote end will receive no     more data (after queued data is flushed). Sockets are automatically closed when they are garbage-collected, but it is           recommended to close() them explicitly.

