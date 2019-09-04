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
