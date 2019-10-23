# RhodeIT-POA-Cluster
Proof of Authority Blockchain Cluster

### Network Structure
- Overview
![Alt text](/Screenshots/2.png)
### Raspberry PI3B
The raspberry PI is used as a client node whos responsibility is to send transaction to the sealer nodes, it acts as a
Bluetooth server at a docking station thus creating a internet of Raspberry PIS who are also responsible for
communicating with the Bluetooth locks to unlock a bicycle when a user rents it out or docks it back at any docking
station

- Basic Architecture
![Alt text](/Screenshots/1.PNG)

### Spinning of a Sealer Node

- launch the startBootNode.bat script
- launch the startGenesis.bat script
- launch the attachGenesis.bat to unlock all local accounts
- launch the startMining.bat script to start the mining process for the genesis node

- The same process applies for Node1



### Spining off a Client Node
To add soon just need to get my english in line


ws connection is enabled on port 12000 to connect to it simply launch a cmd instance and type the following

```
geth attach ws://localhost:12000
```

the same address applie if you wish to connect to it using web3

```
var provider = new Web3.providers.WebsocketProvider(ws://localhost:12000);
var web3 = new Web3(provider);
```
