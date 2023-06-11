## Introduction

Solidity, the primary language for developing smart contracts on blockchain platforms such as Celo, provides features that enable the creation of timed events within contracts. This feature is often used to create contracts that can only be executed after a certain time period has passed, also known as time lock contracts. In this challenge, you are tasked with developing a simple time lock contract.

## Problem Statement

Design a smart contract that represents a simple time lock mechanism with the following requirements:

1. The contract should allow the contract owner to deposit a certain amount of Celo.
2. The contract should prevent withdrawal of the deposited amount until a specified lock-up period has passed.
3. After the lock-up period has passed, only the contract owner should be able to withdraw the full deposited amount.
4. The contract should prevent any other user from withdrawing the deposited amount.

## Hints

- Use `msg.sender` and `msg.value` to handle the deposit.
- Use `now` global variable to track the time of deposit and calculate the end of the lock-up period.
- Use a `require` statement to enforce that only the contract owner can withdraw and only after the lock-up period.
- The `transfer` function can be used to send the contract's balance to the owner.

## Evaluation Criteria

- **Correctness**: The contract should compile without errors and fulfill all the requirements.
- **Readability**: The contract should be well-documented, with comments explaining the code.
- **Testability**: You should also provide examples of how to test each function of the contract.

Remember, handling real assets on a blockchain requires extreme care and extensive testing. This challenge is a simple exercise and doesn’t cover aspects such as security, efficiency, and upgradability, which are essential for a real-world time lock contract.

For a comprehensive understanding of Celo smart contracts and Solidity, please refer to the Celo and Solidity tutorials.

## Submission

Please reply with a link to your PR on GitHub, including your time lock contract. Also, include any notes or comments you think are necessary to understand your design and choices. Lastly, provide a brief explanation about how each function of the contract should be tested.
