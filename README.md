# Supply chain & data auditing

This repository containts an Ethereum DApp that demonstrates a Supply Chain flow between a Seller and Buyer. The user story is similar to any commonly used supply chain process. A Seller can add items to the inventory system stored in the blockchain. A Buyer can purchase such items from the inventory system. Additionally a Seller can mark an item as Shipped, and similarly a Buyer can mark an item as Received.

The DApp User Interface when running should look like...

![truffle test](images/ftc_product_overview.png)

![truffle test](images/ftc_farm_details.png)

![truffle test](images/ftc_product_details.png)

![truffle test](images/ftc_transaction_history.png)


## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

Please make sure you've already installed ganache-cli, Truffle and enabled MetaMask extension in your browser.

```
Give examples (to be clarified)
```

### Installing

> The starter code is written for **Solidity v0.4.24**. At the time of writing, the current Truffle v5 comes with Solidity v0.5 that requires function *mutability* and *visibility* to be specified (please refer to Solidity [documentation](https://docs.soliditylang.org/en/v0.5.0/050-breaking-changes.html) for more details). To use this starter code, please run `npm i -g truffle@4.1.14` to install Truffle v4 with Solidity v0.4.24. 

A step by step series of examples that tell you have to get a development env running

Clone this repository:

```
git clone https://github.com/udacity/nd1309/tree/master/course-5/project-6
```

Change directory to ```project-6``` folder and install all requisite npm packages (as listed in ```package.json```):

```
cd project-6
npm install
```

Launch Ganache:

```
ganache-cli -m "spirit supply whale amount human item harsh scare congress discover talent hamster"
```

Your terminal should look something like this:

![truffle test](images/ganache-cli.png)

In a separate terminal window, Compile smart contracts:

```
truffle compile
```

Your terminal should look something like this:

![truffle test](images/truffle_compile.png)

This will create the smart contract artifacts in folder ```build\contracts```.

Migrate smart contracts to the locally running blockchain, ganache-cli:

```
truffle migrate
```

Your terminal should look something like this:

![truffle test](images/truffle_migrate.png)

Test smart contracts:

```
truffle test
```

All 10 tests should pass.

![truffle test](images/truffle_test.png)

In a separate terminal window, launch the DApp:

```
npm run dev
```

## Built With

* [Ethereum](https://www.ethereum.org/) - Ethereum is a decentralized platform that runs smart contracts
* [IPFS](https://ipfs.io/) - IPFS is the Distributed Web | A peer-to-peer hypermedia protocol
to make the web faster, safer, and more open.
* [Truffle Framework](http://truffleframework.com/) - Truffle is the most popular development framework for Ethereum with a mission to make your life a whole lot easier.


## Authors

See also the list of [contributors](https://github.com/your/project/contributors.md) who participated in this project.

## Acknowledgments

* Solidity
* Ganache-cli
* Truffle
* IPFS





Starting migrations...
======================
> Network name:    'development'
> Network id:      1639609396846
> Block gas limit: 6721975 (0x6691b7)


1_initial_migration.js
======================

   Deploying 'Migrations'
   ----------------------
   > transaction hash:    0xeda039d038ae75c48ace386515121a47997840e3b8939dcb6dc89b43d9cf12af
   > Blocks: 0            Seconds: 0
   > contract address:    0xFEeCfF2CB7d6f3BfcBE5fa41c49c8fB642f2dDbF
   > block number:        1
   > block timestamp:     1639610843
   > account:             0x27D8D15CbC94527cAdf5eC14B69519aE23288B95
   > balance:             99.99549526
   > gas used:            225237 (0x36fd5)
   > gas price:           20 gwei
   > value sent:          0 ETH
   > total cost:          0.00450474 ETH


   > Saving migration to chain.
   > Saving artifacts
   -------------------------------------
   > Total cost:          0.00450474 ETH


2_deploy_contracts.js
=====================

   Deploying 'FarmerRole'
   ----------------------
   > transaction hash:    0x867fe9ff876496f2cc1d506968fdbc26bb35ddd233ca4c4e8d24a36a41ffcf55
   > Blocks: 0            Seconds: 0
   > contract address:    0xf2ee0b0Cdcae5013930B92c0Ba54F7F7f1933613
   > block number:        3
   > block timestamp:     1639610843
   > account:             0x27D8D15CbC94527cAdf5eC14B69519aE23288B95
   > balance:             99.98808148
   > gas used:            328326 (0x50286)
   > gas price:           20 gwei
   > value sent:          0 ETH
   > total cost:          0.00656652 ETH


   Deploying 'DistributorRole'
   ---------------------------
   > transaction hash:    0x481e042d328dc7dcecc66b85ff6b80de6cfbe08ef7dc2874420ab734a05c105e
   > Blocks: 0            Seconds: 0
   > contract address:    0xd22De155853B67cE1cA3693FBE52EE958f755E7b
   > block number:        4
   > block timestamp:     1639610844
   > account:             0x27D8D15CbC94527cAdf5eC14B69519aE23288B95
   > balance:             99.981514
   > gas used:            328374 (0x502b6)
   > gas price:           20 gwei
   > value sent:          0 ETH
   > total cost:          0.00656748 ETH


   Deploying 'RetailerRole'
   ------------------------
   > transaction hash:    0xd2e75d4f8dcb0807a87986d40b45a25a17e7bfeba4ba23de9f4ffe0877f12082
   > Blocks: 0            Seconds: 0
   > contract address:    0x79051A2faFcC216A55d3897474012145d158F170
   > block number:        5
   > block timestamp:     1639610844
   > account:             0x27D8D15CbC94527cAdf5eC14B69519aE23288B95
   > balance:             99.974947
   > gas used:            328350 (0x5029e)
   > gas price:           20 gwei
   > value sent:          0 ETH
   > total cost:          0.006567 ETH


   Deploying 'ConsumerRole'
   ------------------------
   > transaction hash:    0x46a7578ab8b2684967cbc70d1d2f91cce5db5818b36f29d38b2391577e45fbf7
   > Blocks: 0            Seconds: 0
   > contract address:    0xA65B87754E0A73860AA6B7eb6E95D79CD2d893d2
   > block number:        6
   > block timestamp:     1639610844
   > account:             0x27D8D15CbC94527cAdf5eC14B69519aE23288B95
   > balance:             99.96838
   > gas used:            328350 (0x5029e)
   > gas price:           20 gwei
   > value sent:          0 ETH
   > total cost:          0.006567 ETH


   Deploying 'SupplyChain'
   -----------------------
   > transaction hash:    0xcd4b7463d895a1a648639aad364da20880760da5174ebac119dfc9f3fdae11c9
   > Blocks: 0            Seconds: 0
   > contract address:    0x23E2b13b08a22E9eEe431F862eC7A17aB1E99B98
   > block number:        7
   > block timestamp:     1639610845
   > account:             0x27D8D15CbC94527cAdf5eC14B69519aE23288B95
   > balance:             99.90513464
   > gas used:            3162268 (0x30409c)
   > gas price:           20 gwei
   > value sent:          0 ETH
   > total cost:          0.06324536 ETH


   > Saving migration to chain.
   > Saving artifacts
   -------------------------------------
   > Total cost:          0.08951336 ETH


Summary
=======
> Total deployments:   6
> Final cost:          0.0940181 ETH


1vim@Saads-MacBook-Air supply_chain_project-main % truffle test
Using network 'development'.


Compiling your contracts...
===========================
> Everything is up to date, there is nothing to compile.

ganache-cli accounts used here...
Contract Owner: accounts[0]  0x27D8D15CbC94527cAdf5eC14B69519aE23288B95
Farmer: accounts[1]  0x018C2daBef4904ECbd7118350A0c54DbeaE3549A
Distributor: accounts[2]  0xCe5144391B4aB80668965F2Cc4f2CC102380Ef0A
Retailer: accounts[3]  0x460c31107DD048e34971E57DA2F99f659Add4f02
Consumer: accounts[4]  0xD37b7B8C62BE2fdDe8dAa9816483AeBDBd356088


  Contract: SupplyChain
    ✓ Testing smart contract function harvestItem() that allows a farmer to harvest coffee (586ms)
    ✓ Testing smart contract function processItem() that allows a farmer to process coffee (319ms)
    ✓ Testing smart contract function packItem() that allows a farmer to pack coffee (192ms)
    ✓ Testing smart contract function sellItem() that allows a farmer to sell coffee (385ms)
    ✓ Testing smart contract function buyItem() that allows a distributor to buy coffee (356ms)
    ✓ Testing smart contract function shipItem() that allows a distributor to ship coffee (259ms)
    ✓ Testing smart contract function receiveItem() that allows a retailer to mark coffee received (383ms)
    ✓ Testing smart contract function purchaseItem() that allows a consumer to purchase coffee (409ms)
    ✓ Testing smart contract function fetchItemBufferOne() that allows anyone to fetch item details from blockchain (78ms)
    ✓ Testing smart contract function fetchItemBufferTwo() that allows anyone to fetch item details from blockchain (62ms)


  10 passing (3s)

1vim@Saads-MacBook-Air supply_chain_project-main % 




Compiling your contracts...
===========================
> Compiling ./contracts/Migrations.sol
> Compiling ./contracts/coffeeaccesscontrol/ConsumerRole.sol
> Compiling ./contracts/coffeeaccesscontrol/DistributorRole.sol
> Compiling ./contracts/coffeeaccesscontrol/FarmerRole.sol
> Compiling ./contracts/coffeeaccesscontrol/RetailerRole.sol
> Compiling ./contracts/coffeeaccesscontrol/Roles.sol
> Compiling ./contracts/coffeebase/SupplyChain.sol
> Compiling ./contracts/coffeecore/Ownable.sol
> Artifacts written to /Users/1vim/Desktop/supply_chain_project-main/build/contracts
> Compiled successfully using:
   - solc: 0.5.16+commit.9c3226ce.Emscripten.clang



Migrations dry-run (simulation)
===============================
> Network name:    'rinkeby-fork'
> Network id:      4
> Block gas limit: 29970620 (0x1c950bc)


1_initial_migration.js
======================

   Deploying 'Migrations'
   ----------------------
   > block number:        9821020
   > block timestamp:     1639609899
   > account:             0xefa409f8db2dCa2D0d8838ab72CBA15Ffc4e4026
   > balance:             1.5958889285
   > gas used:            210237 (0x3353d)
   > gas price:           10 gwei
   > value sent:          0 ETH
   > total cost:          0.00210237 ETH

   -------------------------------------
   > Total cost:          0.00210237 ETH


2_deploy_contracts.js
=====================

   Deploying 'FarmerRole'
   ----------------------
   > block number:        9821022
   > block timestamp:     1639609902
   > account:             0xefa409f8db2dCa2D0d8838ab72CBA15Ffc4e4026
   > balance:             1.5924820385
   > gas used:            313326 (0x4c7ee)
   > gas price:           10 gwei
   > value sent:          0 ETH
   > total cost:          0.00313326 ETH


   Deploying 'DistributorRole'
   ---------------------------
   > block number:        9821023
   > block timestamp:     1639609905
   > account:             0xefa409f8db2dCa2D0d8838ab72CBA15Ffc4e4026
   > balance:             1.5893482985
   > gas used:            313374 (0x4c81e)
   > gas price:           10 gwei
   > value sent:          0 ETH
   > total cost:          0.00313374 ETH


   Deploying 'RetailerRole'
   ------------------------
   > block number:        9821024
   > block timestamp:     1639609907
   > account:             0xefa409f8db2dCa2D0d8838ab72CBA15Ffc4e4026
   > balance:             1.5862147985
   > gas used:            313350 (0x4c806)
   > gas price:           10 gwei
   > value sent:          0 ETH
   > total cost:          0.0031335 ETH


   Deploying 'ConsumerRole'
   ------------------------
   > block number:        9821025
   > block timestamp:     1639609908
   > account:             0xefa409f8db2dCa2D0d8838ab72CBA15Ffc4e4026
   > balance:             1.5830812985
   > gas used:            313350 (0x4c806)
   > gas price:           10 gwei
   > value sent:          0 ETH
   > total cost:          0.0031335 ETH


   Deploying 'SupplyChain'
   -----------------------
   > block number:        9821026
   > block timestamp:     1639609912
   > account:             0xefa409f8db2dCa2D0d8838ab72CBA15Ffc4e4026
   > balance:             1.5525086185
   > gas used:            3057268 (0x2ea674)
   > gas price:           10 gwei
   > value sent:          0 ETH
   > total cost:          0.03057268 ETH

   -------------------------------------
   > Total cost:          0.04310668 ETH


Summary
=======
> Total deployments:   6
> Final cost:          0.04520905 ETH


Warning: Both truffle-config.js and truffle.js were found. Using truffle-config.js.
Warning: Both truffle-config.js and truffle.js were found. Using truffle-config.js.



Starting migrations...
======================
> Network name:    'rinkeby'
> Network id:      4
> Block gas limit: 29999887 (0x1c9c30f)


1_initial_migration.js
======================

   Deploying 'Migrations'
   ----------------------
   > transaction hash:    0x85e55f561ad9cb56a1e477136202d0120858750e089775ba968e6bb3c24fd3ab
   > Blocks: 0            Seconds: 4
   > contract address:    0x64AE99C1754f4f34725D596648fCd25a375D3525
   > block number:        9821020
   > block timestamp:     1639609921
   > account:             0xefa409f8db2dCa2D0d8838ab72CBA15Ffc4e4026
   > balance:             1.5957259285
   > gas used:            226537 (0x374e9)
   > gas price:           10 gwei
   > value sent:          0 ETH
   > total cost:          0.00226537 ETH


   > Saving migration to chain.
   > Saving artifacts
   -------------------------------------
   > Total cost:          0.00226537 ETH


2_deploy_contracts.js
=====================

   Deploying 'FarmerRole'
   ----------------------
   > transaction hash:    0x183e396dd724b597ed5bb3f9ae333651b0c3c6e8195ee06e5dd9026c8798bbb9
   > Blocks: 0            Seconds: 12
   > contract address:    0xf550CC4988FC944CA2747172FeBE7cb53d739A08
   > block number:        9821022
   > block timestamp:     1639609951
   > account:             0xefa409f8db2dCa2D0d8838ab72CBA15Ffc4e4026
   > balance:             1.5919790385
   > gas used:            328926 (0x504de)
   > gas price:           10 gwei
   > value sent:          0 ETH
   > total cost:          0.00328926 ETH


   Deploying 'DistributorRole'
   ---------------------------
   > transaction hash:    0xad1a4f4cc6bcd8115d5b17255c662dd039e52e3332ccf51eff004f2813bb62f0
   > Blocks: 0            Seconds: 12
   > contract address:    0xBA10880B3adf536342487db4428405f1A3D6d2d5
   > block number:        9821023
   > block timestamp:     1639609966
   > account:             0xefa409f8db2dCa2D0d8838ab72CBA15Ffc4e4026
   > balance:             1.5886892985
   > gas used:            328974 (0x5050e)
   > gas price:           10 gwei
   > value sent:          0 ETH
   > total cost:          0.00328974 ETH


   Deploying 'RetailerRole'
   ------------------------
   > transaction hash:    0xdb2e52daa81f7f999cdbab78d0b7b8d84030fe2fae5c3393278f1d096698d562
   > Blocks: 0            Seconds: 12
   > contract address:    0xd4484b5FB0e0df559e06Bb87275325E38bf12C11
   > block number:        9821024
   > block timestamp:     1639609981
   > account:             0xefa409f8db2dCa2D0d8838ab72CBA15Ffc4e4026
   > balance:             1.5853997985
   > gas used:            328950 (0x504f6)
   > gas price:           10 gwei
   > value sent:          0 ETH
   > total cost:          0.0032895 ETH


   Deploying 'ConsumerRole'
   ------------------------
   > transaction hash:    0x92b7f3d4970786c0dd2f0289187446ca99c2683f5970558cbbafb923345528e5
   > Blocks: 1            Seconds: 16
   > contract address:    0x50B66ee72c5297D0564Bd43d1a5861c89E277E23
   > block number:        9821025
   > block timestamp:     1639609996
   > account:             0xefa409f8db2dCa2D0d8838ab72CBA15Ffc4e4026
   > balance:             1.5821102985
   > gas used:            328950 (0x504f6)
   > gas price:           10 gwei
   > value sent:          0 ETH
   > total cost:          0.0032895 ETH


   Deploying 'SupplyChain'
   -----------------------
   > transaction hash:    0xc0040c6888095a6162c8e6ef6238565be627d30aea55b1ef27801dc73f7f0c5d
   > Blocks: 0            Seconds: 12
   > contract address:    0x012E33AcA39f88FbDA6F5fb2305044456bab423f
   > block number:        9821026
   > block timestamp:     1639610011
   > account:             0xefa409f8db2dCa2D0d8838ab72CBA15Ffc4e4026
   > balance:             1.5504156185
   > gas used:            3169468 (0x305cbc)
   > gas price:           10 gwei
   > value sent:          0 ETH
   > total cost:          0.03169468 ETH


   > Saving migration to chain.
   > Saving artifacts
   -------------------------------------
   > Total cost:          0.04485268 ETH


Summary
=======
> Total deployments:   6
> Final cost:          0.04711805 ETH



