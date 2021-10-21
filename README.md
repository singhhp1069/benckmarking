# Blockchain Benckarking

## Blockchains
* Ethereum
* Cosmos-Starport
* Polkadot-Substrate
* Avalanche
* Solana

## Benchmarking Matrix Problem

**Transactions-per-second** -  very ambiguous and flighty metric. 

The standard TPS parameter for evaluating blockchains is *WRONG*.

**Reasons**
* Transaction per second term came from the distributed databases. And the result of TPS is performed using standard transaction operations (e.g., INSERT, UPDATE, DELETE, SELECT). 
* Configuration of the cluster/machine used for the benchmarking matters.
* Also distributed database trade-off between one of the parameters in CAP Theorem. 
* **Consistency-Oriented Databases** - do not commit the transaction until they receive sufficient confirmation from other nodes - and **this makes a system very slow**. E.g., ACID consistency model DB such as relational databases.
* **Availability-Oriented Database** - consider a transaction successful if it is written to a disk. They immediately provide the updated data - and **this makes a system very fast**. E.g., BASE consistency model DB such as NoSQL.

Blockchain is inherently fault-tolerant by decentralization and methods of achieving consensus. E.g., In **Proof-of-Work (PoW)**, transactions are never finalized at all; if a transaction is included in a blockchain on one machine, this doesn't mean the entire network accepts it.
The existing matrix can't measure the actual performance; even if it does, there will be trade-offs between security, tx finality (centralization), safety, etc.

In this tool, we define key metrics considering the state of the art of blockchains and evaluate various popular blockchains.


## Blockchain Benckmark Matrix


### Local TPS (Tx/sec)


* The number of processed transactions and max/avg/min processing time (on the local node) 
* Transaction processing time is a time which is necessary to update the state database
Many projects claim 10k tps (result are in defined params, local. Without the network influence). This number doesn't reflect the real network bandwidth but shows how fast the consensus and network is.


## Setup Guide

## Results


