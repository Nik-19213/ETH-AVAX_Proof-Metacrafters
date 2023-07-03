# ErrorHandling Contract

This is a Solidity smart contract that demonstrates different error handling techniques using `assert`, `revert`, and `require` functions.

## Prerequisites

- Solidity ^0.8.17
- Remix IDE

## Contract Details

The `ErrorHandling` contract provides the following functions:

### `divide(uint _numerator, uint _denominator)`

- This function demonstrates the usage of the `require` function.
- It takes `_numerator` and `_denominator` parameters and performs division.
- If the `_denominator` is provided zero , then the function terminates and returns the message `Division by zero not possible `.
- If the denominator is not zero , it performs the division.

### `EnterRollNumber(uint _roll)`

- This function demonstrates the usage of the `revert` function.
- It takes a `_roll` parameter and checks if it is equal to zero.
- If the condition is true and roll number is equal to zero it reverts the message `Value of roll number cannot be 0`.
- If the condition is false , it returns the roll number provided. 

### `getElement(uint256 index)`

- This function demonstrates the usage of the `assert` function.
- It takes an `index` parameter and by using essert checks if the index number is less than the length of array.
- If the condition is true and index is less than the length of array it returns the value of element at that index.

## Usage

1. Make sure you have Solidity ^0.8.17 installed.
2. Compile and deploy the `ErrorHandling` contract to a supported Ethereum network.
3. Interact with the deployed contract by calling the available functions and providing the required parameters.

## License

This contract is using the SPDX-License-Identifier: GPL-3.0
