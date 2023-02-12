# Unit 20 - "Joint Savings Account"

![alt=“”](Images/20-5-challenge-image.png)

### Background

A fintech startup company has recently hired you. This company is disrupting the finance industry with its own cross-border, Ethereum-compatible blockchain that connects financial institutions. Currently, the team is building smart contracts to automate many of the institutions’ financial processes and features, such as hosting joint savings accounts.

To automate the creation of joint savings accounts, you’ll create a Solidity smart contract that accepts two user addresses. These addresses will be able to control a joint savings account. Your smart contract will use ether management functions to implement a financial institution’s requirements for providing the features of the joint savings account. These features will consist of the ability to deposit and withdraw funds from the account.

# Execution Results
After each step, a screenshot of the execution is captured and  saved to a folder named `Execution_Results`. 

>   Account Address:
    0x5B38Da6a701c568545dCfcB03FcB875f56beddC4

![alt=“”](Execution_Results/initial-info-after-deploying.png)


Execution steps:

1. Use the `setAccounts` function to define the authorized Ethereum address that will be able to withdraw funds from your contract.

   >  Dummy account1 address: 0x0c0669Cd5e60a6F4b8ce437E4a4A007093D368Cb

   >  Dummy account2 address: 0x7A1f3dFAa0a4a19844B606CD6e91d693083B12c0

![alt=“”](Execution_Results/set-account1-and-account2.png)


2. Test the deposit functionality of your smart contract by sending the following amounts of ether. After each transaction, use the `contractBalance` function to verify that the funds were added to your contract:

    * Transaction 1: Send 1 ether as wei.

        Step1: Set the Value to 1 ETH
    ![alt=“”](Execution_Results/deposit-1eth.png)

        Step2: Execute Deposit Function
    ![alt=“”](Execution_Results/deposit-1eth-2.png)
        
        Step3: Contract Balance Check

    ![alt=“”](Execution_Results/deposit-1eth-contractBalance.png)
git
    * Transaction 2: Send 10 ether as wei.

        Step1: Set the Value to 10 ETH
    ![alt=“”](Execution_Results/deposit-10eth-1.png)
        Step2: Execute Deposit Function
    ![alt=“”](Execution_Results/deposit-10eth-2.png)

        Step3: Contract Balance Check
    ![alt=“”](Execution_Results/deposit-10eth-3.png)

    * Transaction 3: Send 5 ether.
        Step1: Set the Value to 5 ETH
    ![alt=“”](Execution_Results/deposit-5eth-1.png)

        Step2: Execute Deposit Function
    ![alt=“”](Execution_Results/deposit-5eth-2.png)
        Step3: Contract Balance Check
    ![alt=“”](Execution_Results/deposit-5eth-3.png)

3. Once you’ve successfully deposited funds into your contract, test the contract’s withdrawal functionality by withdrawing 5 ether into `accountOne` and 10 ether into `accountTwo`. After each transaction, use the `contractBalance` function to verify that the funds were withdrawn from your contract. Also, use the `lastToWithdraw` and `lastWithdrawAmount` functions to verify that the address and amount were correct.

    * Withdraw 5ETH into Account1
    ![alt=“”](Execution_Results/withdraw-5eth-into-account1.png)

    * Check the Contact Balance using contractBalance function to verify that the funds were withdrawn from the contract
    ![alt=“”](Execution_Results/withdraw-5eth-contract-balance.png)

    * Verify that the address is correct using lastToWithdraw
    ![alt=“”](Execution_Results/withdraw-5eth-lastToWithdraw.png)

    * Verify that the amount is correct using lastWithdrawAmount
    ![alt=“”](Execution_Results/withdraw-5eth-lastWithdrawAmount.png)

    * Withdraw 10ETH into Account2
    ![alt=“”](Execution_Results/withdraw-10eth-into-account2.png)

    * Check the Contact Balance using contractBalance function to verify that the funds were withdrawn from the contract
    ![alt=“”](Execution_Results/withdraw-10eth-contract-balance.png)

    * Verify that the address is correct using lastToWithdraw
    ![alt=“”](Execution_Results/withdraw-10eth-lastToWithdraw.png
)

    * Verify that the amount is correct using lastWithdrawAmount
    ![alt=“”](Execution_Results/withdraw-10eth-lastWithdrawAmount.png)


---
12-Feb-2023

