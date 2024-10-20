# Steps to run the project:

1. Make a .env file in the root of the project
2. To get fake ethers for sepolia testnet go to https://cloud.google.com/application/web3/faucet/ethereum/sepolia and follow the instructions
3. got to https://dashboard.alchemy.com/
4. Make your account in alchemy. After making account you will get a api key.Copy that
5. Go to .env and put an environment variable: GOERLI_URL="https://eth-sepolia.g.alchemy.com/v2/<Your_Api_Key>"
6. In metamask make sure you are on sepolia network. You can change network from top left dropdown. Click on enable testnet and search sepolia there
7. Go to your metamask account. Click on the account dropdown at top and then the three dots. From there you can get your private key
8. Go to .env and create an environment variable PRIVATE_KEY="<YOUR_PRIVATE_KEY>"
9.  run npm i in the root directory and then cd into `client` and then do npm i again
10. Come into root directory type `npx hardhat run scripts/deploy.js --networks sepolia`. This will give the address where your smart contract is deployed on sepolia copy that and got to App.jsx and paste it in `const contractAddres="<YOUR_ADDRESS>";`
11. Go to sepolia.etherscan.io and paste your smart contract address in the search bar. Your deployed smart contract should show up
12. cd into client and run npm run dev
