
## Negotiate peer connection

Client A                                  Client B
--------                                  --------
Broadcast self    ======================> Scan for peer
Receive request   <---------------------- Send connect request
Accept request
Generate TLS
Send TLS certs    ======================> Receive TLS certs
                                          Accept TLS certs
                                          Generate TLS
Receive TLS certs <---------------------- Send TLS certs
Accept TLS certs



### Broadcast self
  Peer multicasts availability to the local network

### Scan for peer
  Peer is listening for multicasts from another peer

### Send connect request
  After a peer recieves a multicast connection, the peer sends back a
  connection request.  The connection request is used to start the
  establishment of a secure connection between the two peers.




