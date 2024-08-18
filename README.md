# Decentralized Voting Application

This is a demo application to implement voting in solidity smart contract using ReactJS. 

[Youtube Tutorial](https://youtu.be/eCn6mHTpuM0)

## Installation

After you cloned the repository, you want to install the packages using

```shell
npm install
```

You first need to compile the contract and upload it to the blockchain network. Run the following commands to compile and upload the contract.

```shell
npx hardhat compile
npx hardhat run --network volta scripts/deploy.js
```

Once the contract is uploaded to the blockchain, copy the contract address and copy it in the .env file. You can also use another blockchain by writing the blockchain's endpoint in hardhat-config.

Once you have pasted your private key and contract address in the .env file, simply run command

```shell
npm start
```
1. clone the repo
2. go into the folder, install the packages using npm install
3. create an .env file with API_URL (testnet url) and your metamaks account's private key (specified later)
4. run "npx hardhat compile"
5. run "npx hardhat run --network volta scripts/deploy.js" to get a contract address. Update this in src/constant/constant.js for every deployment.
6. run npm start
7. set up your metamask wallet and make sure there are enough funds in it. If there are no funds, go to https://voltafaucet.energyweb.org/ to request for dummy tokens on volta network.
8. in the website, login to your metamask wallet and cast your vote.
9. check different accounts to make sure voting is happening properly
10. to check transaction status, go to https://volta-explorer.energyweb.org/txs?block_number=28967466&index=4&page_number=1&page_size=50&pages_limit=200
