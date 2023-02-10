# Unit 20 - "Joint Savings Account"

![alt=“”](Images/20-5-challenge-image.png)

### Background

A fintech startup company has recently hired you. This company is disrupting the finance industry with its own cross-border, Ethereum-compatible blockchain that connects financial institutions. Currently, the team is building smart contracts to automate many of the institutions’ financial processes and features, such as hosting joint savings accounts.

To automate the creation of joint savings accounts, you’ll create a Solidity smart contract that accepts two user addresses. These addresses will be able to control a joint savings account. Your smart contract will use ether management functions to implement a financial institution’s requirements for providing the features of the joint savings account. These features will consist of the ability to deposit and withdraw funds from the account.

# Execution Results
After each step, a screenshot of the execution is captured and  saved to a folder named `Execution_Results`. 

>   Account Address:
    0x617F2E2fD72FD9D5503197092aC168c91465E7f2

![alt=“”](Execution_Results/initial-screenshot-after-deploying.png)


Execution steps:

1. Use the `setAccounts` function to define the authorized Ethereum address that will be able to withdraw funds from your contract.

   >  Dummy account1 address: 0x0c0669Cd5e60a6F4b8ce437E4a4A007093D368Cb

   >  Dummy account2 address: 0x7A1f3dFAa0a4a19844B606CD6e91d693083B12c0

![alt=“”](Execution_Results/set-account1-and-account2.png)


2. Test the deposit functionality of your smart contract by sending the following amounts of ether. After each transaction, use the `contractBalance` function to verify that the funds were added to your contract:

    * Transaction 1: Send 1 ether as wei.
![alt=“”](Execution_Results/deposit-1eth.png)

    * Transaction 2: Send 10 ether as wei.
    ![alt=“”](Execution_Results/deposit-10eth-1.png)

    ![alt=“”](Execution_Results/deposit-10eth-2.png)

    * Transaction 3: Send 5 ether.
    ![alt=“”](Execution_Results/deposit-5eth-1.png)
    ![alt=“”](Execution_Results/deposit-5eth-2.png)


3. Once you’ve successfully deposited funds into your contract, test the contract’s withdrawal functionality by withdrawing 5 ether into `accountOne` and 10 ether into `accountTwo`. After each transaction, use the `contractBalance` function to verify that the funds were withdrawn from your contract. Also, use the `lastToWithdraw` and `lastWithdrawAmount` functions to verify that the address and amount were correct.






---
7-Feb-2023

