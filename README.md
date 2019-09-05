# go-pika

Go lang implementation of pikachain. GO PIKA PIKA!

Experimental code. Heavy WIP!  
** **NOT FOR PRODUCTION** **

## Structure

The project is structured into several modules based on the new functionalities being experimented here:

`cmd`: To handle the CLI arguments, parameters, input/output operations of the POC.

`common`: To persist common variables and info required by almost every other module in the project.

`core`: To facilitates the main logic such as type definitions, formal verification, block characterization and block production.

`p2pnet`: This is a *functional module* to handle the transaction in p2p fashion among all the nodes in the POC network.

`wavm`: This is another *functional module* responsible for executing all the transactional requests in the WASM environment.

`consensus`: This is also another *functional module* to solve the consensus problem once a block is produced.

`log`: To log all the operations(front+backend) of the POC. Duh.

## Objectives of this POC

### Blockchain

1. Create a basic PoS blockchain (list of blocks linked by cryptographic signature) integrating the new innovation in networking, computation and consensus.

### Networking

1. Implement and expose services using libp2p through APIs and RPCs so that multiple instances can communicate with each other (allow our instances to form a blockchain network)

### Computation

1. Facilitate a WASM runtime for the execution of simple arithmetic logic across the network.

### Consensus

1. Implement a simple PoS based consensus algorithm(let our instances agree on shared state)
