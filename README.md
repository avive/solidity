# Getting started with Solidity development - OS X

## Solidity Language Learning

### docs
Read all the pages, twice: https://solidity.readthedocs.io/en/develop/  
https://www.youtube.com/watch?v=8jI1TuEaTro  

### Blogs & Guides
https://github.com/fivedogit/solidity-baby-steps/tree/master/contracts/  
https://www.ethereum.org/token    
https://www.ethereum.org/crowdsale  
https://www.ethereum.org/dao  
https://medium.com/zeppelin-blog/the-hitchhikers-guide-to-smart-contracts-in-ethereum-848f08001f05  
https://hackernoon.com/getting-started-as-an-ethereum-web-developer-9a2a4ab47baf  
https://github.com/ConsenSys/Tokens
https://github.com/ConsenSys/MultiSigWallet

### Forums & Community
https://ethereum.stackexchange.com/  
https://gitter.im/ethereum/home  
https://www.reddit.com/r/ethereum/  
https://stackoverflow.com/questions/tagged/ethereum  

### Dapps open source examples
https://github.com/ethereum/dapp-bin  
https://github.com/ethereum/dapp-bin/tree/master/getting%20started  

## Dev tools - OS X

### geth
https://geth.ethereum.org/  
```
$ brew tap ethereum/ethereum    
$ brew install ethereum  
$ geth --version  
```

### solcjs
```
$ npm install -g solc 
$ solcjs --version
```

### solc
http://solidity.readthedocs.io/en/develop/installing-solidity.html  
Follow instructions to build from source  
```
$ solc --version  
```

### Truffle
https://github.com/trufflesuite/truffle  
```
$ npm install -g truffle
$ cd <new-project-folder>
$ truffle init
```

### Dapple
https://github.com/dapphub/dapple   

### Webpack-based dev seed
https://github.com/uzyn/ethereum-webpack-example-dapp  

### Testrpc
https://github.com/ethereumjs/testrpc  
```
$ sudo npm install -g ethereumjs-testrpc
$ testrpc
```

* Testrpc dcoker
```
$ docker run -d -p 8545:8545 ethereumjs/testrpc:latest
```

### Intellij-Solidity syntax support
https://plugins.jetbrains.com/plugin/9475-intellij-solidity  

### Remix
https://github.com/ethereum/remix  

```
$ git clone https://github.com/ethereum/remix
$ cd remix
$ npm install
$ npm start
```

### Debugging, Logging & Events

### Test Networks

Rinkeby (modern)  
https://www.rinkeby.io/  -> connect yourself  
Download the json file and follow the instructions  

### Running geth in a docker container
https://github.com/ethereum/go-ethereum/wiki/Running-in-Docker

## Basic Concepts
* contract
* account types - external or contract. Has an address and a balance. External accounts have key paris
* transactions - tpyes: contract creation, move funds to an account, call a contract method
* message calls - calldata area, used in transactions
* delegate calls - using caller context for library / util functions
* Gas - gas price and gas amount set by transaction initiator. Used for code execution
* Events
* EVM - stack-based machine, contract storage and memory (runtime env)
* throw
* Suicide
* Get block number
* Constant fucntions
* Obtaining contract address
* Global variables - msg, tx, block
* Getting call data from the Message global var - msg.value, msg.sender, msg.data
* Working with transactions - tx.*  
* Working with Gas - msg.gas,  tx.gasprice - gas caller is willing to pay  
* this === address
* The unamed function with optional payability

## Security Considirations and Best Practices
https://solidity.readthedocs.io/en/develop/security-considerations.html
https://github.com/ethereum/dapp-bin/tree/master/standardized_contract_apis  

* Beware of external contracts calls - they can call back to your contract and change its control flow
* Private data is viewable by anyone
* All your public contract methods may be called maliciously
* Bug bounty hunt your contracts on a test network and perform security audits with highly reputable 3rd parties

## Solidity Design Patterns
https://github.com/ConsenSys/smart-contract-best-practices

### Testing Patterns
* Testing with testrpc
* Testing with testrpc and truffle
```
https://github.com/ethereumjs/testrpc
http://truffleframework.com/docs/getting_started/javascript-tests
```

* Testing a private test network
* Testing with a public testnet
* Security audits options
* Testing with docker
https://github.com/Capgemini-AIE/ethereum-docker  

### Factory Pattern
A contract for registration of contract addresses deployed by an external account address   

### Enahnced Security with Multi-sig Wallets

### Payments Lockout Pattern

### Auction Patterns

### Crowd Funding Patterns

### The Withdraw Pattern
* Don't send money - let other widthdraw what they are authorized to get

### Working with time
* block.timestamp === Now() - epoch time in secs  
* Block ids as time units
* Other options for time-based operations

### Design Patterns Resources
https://github.com/ethereum/wiki/wiki/Useful-%C3%90app-Patterns  
https://github.com/ConsenSys/Ethereum-Development-Best-Practices/wiki/Dapp-Architecture-Designs  
https://www.youtube.com/watch?v=XkJ8mg-R7C0  
https://github.com/ConsenSys/gnosis-contracts  
https://github.com/ConsenSys  
https://github.com/toadkicker/solidity-patterns  

## Data Structures and Utils

### Built-in data structures
* structs
* mappings
* state vars

### Additional data structures
https://github.com/ethereum/dapp-bin/tree/master/library  

#### key-value store patterns
https://github.com/ConsenSys/dapp-store-contracts  

### Classic Contracts

### Milti-sig Wallets

### Circut Breakers
Designing for failure and worse-case scenarios

### Risk Management
* Rate limiting
* Max usage / Lockouts

### Crowd Funding Campaigns - design and implementation examples
Golem Campaign    
https://blog.golemproject.net/the-golem-crowdfunding-summary-8a3504375aa7  
https://blog.golemproject.net/gnt-crowdfunding-contract-in-pictures-d6b5a2e69150  
https://github.com/golemfactory/golem-crowdfunding  
https://github.com/ConsenSys/dapp-store-contracts  

## Block Explorers & Network Stats
https://etherchain.org/  
https://ethstats.net/  
https://live.ether.camp/  
https://etherscan.io/  

## Disassembliy and Decompilers
https://etherscan.io/opcode-tool?a=0x9e1b57fc92eba6434251a8458811c32690f32c45  
