# Supply chain & data auditing

This repository containts an Ethereum DApp that demonstrates a Supply Chain flow between a Seller and Buyer. The user story is similar to any commonly used supply chain process. A Seller can add items to the inventory system stored in the blockchain. A Buyer can purchase such items from the inventory system. Additionally a Seller can mark an item as Shipped, and similarly a Buyer can mark an item as Received.

## Contract Addresses (Ropsten network)

- FarmerRole: [0x8947C8FECeEeCbCbFc817969e354019F46C49cDB](https://ropsten.etherscan.io/address/0x8947C8FECeEeCbCbFc817969e354019F46C49cDB)
- DistributorRole: [0x86f7bEa2eB874b0eeB792a75f358bcf2f25Bb827](https://ropsten.etherscan.io/address/0x86f7bEa2eB874b0eeB792a75f358bcf2f25Bb827)
- RetailerRole: [0x72bb46DB222083a7Eb9BECdd1CDf934CeAf38a13](https://ropsten.etherscan.io/address/0x72bb46DB222083a7Eb9BECdd1CDf934CeAf38a13)
- ConsumerRole: [0x0ed8a38E57017aC02D4B0c857dCE02Dc34D330F1](https://ropsten.etherscan.io/address/0x0ed8a38E57017aC02D4B0c857dCE02Dc34D330F1)
- SupplyChain: [0xbbFeA30C722AF9122e45C0D6Ecb81Dd574F381F5](https://ropsten.etherscan.io/address/0xbbFeA30C722AF9122e45C0D6Ecb81Dd574F381F5)

## Libraries

- Truffle (v5.1.32) - To develop,test and deploy smart contracts.
- truffle-hdwallet-provider (v1.0.17) - Use it to sign transactions for addresses derived from a 12-word mnemonic.
- yarn (v1.22.4) - Fast, reliable, and secure dependency node manager.

## Project write-up

### Activity

![activity](images/uml_activity.png)

### Sequence

![sequence](images/uml_sequence.png)

### State

![state](images/uml_state.png)

### Class

![class](images/uml_class.png)

## Deployment

```
truffle(ropsten)> truffle deploy --network ropsten --reset

Compiling your contracts...
===========================
> Everything is up to date, there is nothing to compile.



Starting migrations...
======================
> Network name:    'ropsten'
> Network id:      3
> Block gas limit: 0x7a121d


1_initial_migration.js
======================

   Replacing 'Migrations'
   ----------------------
   > transaction hash:    0x3f0009e914a345fd9986865932409da8a7e7de836e10b1b16e8a40150691e9e0
   > Blocks: 1            Seconds: 12
   > contract address:    0x7ea8900CE9a9D464eB5eE5Ab8966Ce56B8A99550
   > block number:        8333074
   > block timestamp:     1595261927
   > account:             0x28d06E693F5fbA5C8821cD6Ebf2f5245DCb6bfB6
   > balance:             5.819363329
   > gas used:            225237
   > gas price:           20 gwei
   > value sent:          0 ETH
   > total cost:          0.00450474 ETH

   Pausing for 2 confirmations...
   ------------------------------
   > confirmation number: 1 (block: 8333075)
   > confirmation number: 2 (block: 8333076)

   > Saving migration to chain.
   > Saving artifacts
   -------------------------------------
   > Total cost:          0.00450474 ETH


2_deploy_contracts.js
=====================

   Replacing 'FarmerRole'
   ----------------------
   > transaction hash:    0x3cfda2c21c75e2a356e7c90e7d351d4f4f88d6989f09329f17e41797e52f30be
   > Blocks: 1            Seconds: 36
   > contract address:    0x8947C8FECeEeCbCbFc817969e354019F46C49cDB
   > block number:        8333079
   > block timestamp:     1595261978
   > account:             0x28d06E693F5fbA5C8821cD6Ebf2f5245DCb6bfB6
   > balance:             5.811951709
   > gas used:            328218
   > gas price:           20 gwei
   > value sent:          0 ETH
   > total cost:          0.00656436 ETH

   Pausing for 2 confirmations...
   ------------------------------
   > confirmation number: 1 (block: 8333080)
   > confirmation number: 2 (block: 8333081)

   Replacing 'DistributorRole'
   ---------------------------
   > transaction hash:    0x4e5d284f88052bd801ab71dc3853d41f4f8e81acc315e9fe8627765fc262ce51
   > Blocks: 1            Seconds: 16
   > contract address:    0x86f7bEa2eB874b0eeB792a75f358bcf2f25Bb827
   > block number:        8333083
   > block timestamp:     1595262090
   > account:             0x28d06E693F5fbA5C8821cD6Ebf2f5245DCb6bfB6
   > balance:             5.805386389
   > gas used:            328266
   > gas price:           20 gwei
   > value sent:          0 ETH
   > total cost:          0.00656532 ETH

   Pausing for 2 confirmations...
   ------------------------------
   > confirmation number: 1 (block: 8333084)
   > confirmation number: 2 (block: 8333085)

   Replacing 'RetailerRole'
   ------------------------
   > transaction hash:    0x4bdb034dcd7c481e57b05c4f594c5de9f6819ddae6b7a3723a2274077921bdae
   > Blocks: 1            Seconds: 44
   > contract address:    0x72bb46DB222083a7Eb9BECdd1CDf934CeAf38a13
   > block number:        8333087
   > block timestamp:     1595262184
   > account:             0x28d06E693F5fbA5C8821cD6Ebf2f5245DCb6bfB6
   > balance:             5.798821789
   > gas used:            328230
   > gas price:           20 gwei
   > value sent:          0 ETH
   > total cost:          0.0065646 ETH

   Pausing for 2 confirmations...
   ------------------------------
   > confirmation number: 1 (block: 8333088)
   > confirmation number: 2 (block: 8333089)

   Replacing 'ConsumerRole'
   ------------------------
   > transaction hash:    0xb5ccd5dc4d2e1ed956bd331b12899ff1a3e21fc1eb56482f848a3baaa5efb897
   > Blocks: 0            Seconds: 20
   > contract address:    0x0ed8a38E57017aC02D4B0c857dCE02Dc34D330F1
   > block number:        8333090
   > block timestamp:     1595262229
   > account:             0x28d06E693F5fbA5C8821cD6Ebf2f5245DCb6bfB6
   > balance:             5.792256949
   > gas used:            328242
   > gas price:           20 gwei
   > value sent:          0 ETH
   > total cost:          0.00656484 ETH

   Pausing for 2 confirmations...
   ------------------------------
   > confirmation number: 1 (block: 8333091)
   > confirmation number: 2 (block: 8333092)

   Replacing 'SupplyChain'
   -----------------------
   > transaction hash:    0x8e2e23120ce2f577496e21a9359ce054d0f75662fe6f643774505726d610ad86
   > Blocks: 2            Seconds: 16
   > contract address:    0xbbFeA30C722AF9122e45C0D6Ecb81Dd574F381F5
   > block number:        8333095
   > block timestamp:     1595262273
   > account:             0x28d06E693F5fbA5C8821cD6Ebf2f5245DCb6bfB6
   > balance:             5.730529669
   > gas used:            3086364
   > gas price:           20 gwei
   > value sent:          0 ETH
   > total cost:          0.06172728 ETH

   Pausing for 2 confirmations...
   ------------------------------
   > confirmation number: 1 (block: 8333096)
   > confirmation number: 2 (block: 8333097)

   > Saving migration to chain.
   > Saving artifacts
   -------------------------------------
   > Total cost:           0.0879864 ETH


Summary
=======
> Total deployments:   6
> Final cost:          0.09249114 ETH
```
