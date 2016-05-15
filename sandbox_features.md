# Sandbox features

'Sandbox' is a node js module that emulates the ethereum network. Once you have a solidity contract code written and saved with .sol suffix, you can run the contract (deploy)it to the sandbox for testing.

![](Ether-Studio-screen2.png)
1. Shown here is the screen an example: the wallet.sol multi signature wallet solidity contract. 
2. Ethereum console shows the output log of transactions
3. The pop-up appears when we run the sandbox (see item #6). The pop-up is the contract constructor allowing you (contract owner) to set the parameters for the creation of the contract and its deployment on the blockchain (sandbox or the live ethereum blockchain). In this specific case, wallet contract needs address(es) of the wallet owner(s), amount of ether held, and daily spend limit.
4. The sandbox panel: lists account addresses and deployed contracts on the sandbox simulated blockchain.
5. The project directory structure. The wallet example project has a directory structure typical of node.js express framework with bower and gulp files for front end / node.js server development. 
6. Run contract(s) / stop sandbox button.
7. 
