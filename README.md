# Steps to run the project:

## Make a .env file in the root of the project
## To get fake ethers for sepolia testnet go to https://cloud.google.com/application/web3/faucet/ethereum/sepolia and follow the instructions
## got to https://dashboard.alchemy.com/
## Make your account in alchemy. After making account you will get a api key.Copy that
## Go to .env and put an environment variable: GOERLI_URL="https://eth-sepolia.g.alchemy.com/v2/<Your_Api_Key>"
## In metamask make sure you are on sepolia network. You can change network from top left dropdown. Click on enable testnet and search sepolia there
## Go to your metamask account. Click on the account dropdown at top and then the three dots. From there you can get your private key
## Go to .env and create an environment variable PRIVATE_KEY="<YOUR_PRIVATE_KEY>"
##  run npm i in the root directory and then cd into `client` and then do npm i again
## Come into root directory type `npx hardhat run scripts/deploy.js --networks sepolia`. This will give the address where your smart contract is deployed on sepolia copy that and got to App.jsx and paste it in `const contractAddres="<YOUR_ADDRESS>";`
## Go to sepolia.etherscan.io and paste your smart contract address in the search bar. Your deployed smart contract should show up
## cd into client and run npm run dev
