#ExceptionExample Contract


#Overview


This repository contains the smart contract code for the ExceptionExample contract. The contract demonstrates the usage of require(), assert(), and revert() statements to handle conditions and ensure the desired behavior of the contract.

#Contract Details


Solidity Version: 0.8.18
License: MIT


#Functionalities


In this contract, we have four functions: deposit(), withdraw(), unsafeWithdraw(), and failedWithdraw(). 

#deposit

The deposit() function allows users to deposit a specified amount into their account. It uses the require() statement to check if the amount is greater than zero before updating the balance variable. 

#withdraw

The withdraw() function allows users to withdraw a specified amount from their account. It uses the require() statement to check if the amount is greater than zero and if it's less than or equal to the current balance. If the conditions are met, it updates the balance variable.

#unsafeWithdraw

The unsafeWithdraw() function demonstrates the usage of assert() statements. It assumes that the inputs have already been validated elsewhere, and therefore it uses assert() to validate the inputs directly. If the conditions specified in the assert() statements are not met, it will result in a runtime error. 


#failedWithdraw

The failedWithdraw() function shows an example of using the revert() statement. It performs the same checks as the withdraw() function but intentionally fails by calling revert() with a custom error message. This will revert the transaction and provide an error message to the caller.

#Deployment and Usage


To deploy the contract, follow these steps:

Compile the smart contract code using a Solidity compiler (e.g., Remix, Truffle).
Deploy the contract to an Ethereum network of your choice (e.g., local development network, public testnet, or mainnet) using a compatible Ethereum client or development framework (e.g., Remix, Truffle, Hardhat).
Development Environment
The contract is developed using Solidity version 0.8.18. It is recommended to use a compatible Solidity compiler or development framework (e.g., Remix, Truffle) for compilation and deployment.

#License


This project is licensed under the MIT License.
