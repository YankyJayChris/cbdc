*This repository is work in progress*
# A Prototype for a Central Bank Digital Currency with Support for Cash-Like Privacy
This prototype implements a subset of the features of the CBDC proposal by [Matthias Babel](https://www.linkedin.com/in/matthiasbabel/), [Alexander Bechtel](https://www.linkedin.com/in/alexanderbechtel/), [Jonas Gross](https://www.linkedin.com/in/jonasgross94/), [Benjamin Schellinger](https://www.linkedin.com/in/benjamin-schellinger-a35684125/), and [Johannes Sedlmeir](https://www.linkedin.com/in/johannes-sedlmeir/).

So far, the prototype implements the Merkle-tree for storing the commitments, a list for the nullifiers, and the basics for 
account and transaction management. In addition, it supports fully private transactions while respecting 
account transaction limits, ensuring compliance by design.

This is achieved by implementing generic zero-knowledge proofs (zk-SNARKs) using the iden3 libraries [circom](https://github.com/iden3/circom) and [snarkjs](https://github.com/iden3/snarkjs).

For information on how zero-knowledge proofs work, https://github.com/matter-labs/awesome-zero-knowledge-proofs is an *awesome* source of material. 

The academic paper is available [here](insert link to SSRN).

## Roadmap
- SSI-based onboarding
- Semi-private transactions

## Install
- Install nodejs(@v16.0.0) and npm (@7.10.0) (for instructions, see, e.g., https://heynode.com/tutorial/install-nodejs-locally-nvm/)
- Clone this repository ``git clone https://github.com/applied-crypto/cbdc``
- Go to cbdc ``cd cbdc``
- Install dependencies ``npm install``
- Run an example transaction: ``node test.js``

