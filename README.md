# Requirements
* Python 2.7.x
* Twisted (a recent version)

## mdht 
A library with implementations of a kademlia node supporting "Mainline DHT".
Written on a Twisted stack.
Protocol spec: http://www.bittorrent.org/beps/bep_0005.html)

### Unit tests
On a shell with a proper PYTHONPATH, do: 'trial mdht.test'

### Protocols
mdht.protocols.krpc_simple:
    "get" and "put" operations

## mdht_server 
A Twisted application that starts up a server with an mdht node and rpc.
Please see the source of mdht_server/app.tac and mdht_server/server.

### To run
```
cd mdht_server
chmod +x server
./server
```

## mdht_client 
An RPC client that connects to an mdht_server.
Please see the source of mdht_client/client.

### To run
```
cd mdht_client
chmod +x client
./client
```

----------
Comments, questions, and patches welcome: gsk067@gmail.com
