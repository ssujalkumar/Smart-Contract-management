This project implements an Ethereum-based ATM where users can deposit and withdraw ETH. The system consists of a smart contract deployed on the Ethereum blockchain and a frontend interface to interact with the contract. The frontend uses MetaMask for user authentication and transaction signing.

Table of Contents
Smart Contract
Frontend
Deployment
Usage
Dependencies
Smart Contract
The smart contract is written in Solidity and allows only the contract owner to deposit and withdraw ETH. Below is a detailed explanation of the contract.

Contract: ATM
State Variables
owner: The owner of the contract.
balance: The balance of ETH in the ATM.
Events
Deposit(uint256 amount): Emitted when ETH is deposited.
Withdraw(uint256 amount): Emitted when ETH is withdrawn.

Frontend
The frontend is built using React and allows users to connect their MetaMask wallet, view their balance, and perform deposit and withdrawal operations.

Components and Functions
HomePage: The main component of the frontend.
getWallet(): Checks if MetaMask is installed and gets the user's wallet.
handleAccount(account): Handles the connected account.
connectAccount(): Connects the user's MetaMask account.
getATMContract(): Gets a reference to the deployed ATM contract.
getBalance(): Fetches the current balance from the contract.
deposit(): Deposits 1 ETH into the contract.
withdraw(): Withdraws 1 ETH from the contract.
UI
The UI displays the connected account and the balance, with buttons to deposit and withdraw ETH.

Deployment
To deploy the smart contract, use the Hardhat framework.

Dependencies
Solidity
Hardhat
Ethers.js
React
MetaMask
