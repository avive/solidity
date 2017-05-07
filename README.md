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
`$ brew tap ethereum/ethereum`  
`$ brew install ethereum`  
`$ geth --version`  

### solcjs
`$ npm install -g solc`  
`$ solcjs --version`  

### solc
http://solidity.readthedocs.io/en/develop/installing-solidity.html  
Follow instructions to build from source  
`$ solc --version`  

### Truffle
https://github.com/trufflesuite/truffle  
`$ npm install -g truffle`  
'$ cd <new-project-folder>`  
`$ truffle init`  

### Dapple
https://github.com/dapphub/dapple   

### Webpack-based dev seed
https://github.com/uzyn/ethereum-webpack-example-dapp  

### Testrpc
https://github.com/ethereumjs/testrpc  
`$ sudo npm install -g ethereumjs-testrpc`  
`$ testrpc`  

### Intellij-Solidity syntax support
https://plugins.jetbrains.com/plugin/9475-intellij-solidity  

### Remix
https://github.com/ethereum/remix  
`$ git clone https://github.com/ethereum/remix`  
`$ cd remix`  
`$ npm install`  
`$ npm start`  

### Debugging, Logging & Events

### Test Networks

Rinkeby (modern)  
https://www.rinkeby.io/  -> connect yourself  
Download the json file and follow the instructions  

## Security Considirations

https://solidity.readthedocs.io/en/develop/security-considerations.html


## Solidity Design Patterns

### Built-in Basic Patterns and Objects
* Suicide
* Get block number
* Constant fucntions
* Obtaining contract address
* Getting call data from the Message object - msg.value, msg.sender, msg.data
* Working with transactions - tx.*  
* Working with Gas - msg.gas,  tx.gasprice - gas caller is willing to pay  
* 


https://github.com/ethereum/dapp-bin/tree/master/standardized_contract_apis  

### Testing Patterns
* Testing with testrpc
* Testing a private test network
* Testing with a public testnet
* Security audits options

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

### Additional data structures
https://github.com/ethereum/dapp-bin/tree/master/library  

#### key-value store patterns
https://github.com/ConsenSys/dapp-store-contracts  

### Classic Contracts

### Milti-sig Wallets

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







