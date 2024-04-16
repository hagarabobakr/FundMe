# FundMe Smart Contract

Welcome to the FundMe smart contract repository! This README provides an overview of the smart contract code and its functionalities.

## Table of Contents

1. [Introduction](#introduction)
2. [PriceConverter Library](#priceconverter-library)
3. [FundMe Contract](#fundme-contract)
4. [Usage](#usage)
5. [Contributing](#contributing)
6. [License](#license)

## Introduction

The FundMe smart contract is designed to allow users to contribute funds to a project. It includes a conversion mechanism to ensure that the contributed amount meets a minimum threshold in USD value.

## PriceConverter Library

The PriceConverter library provides functions for retrieving the price of Ethereum in USD and converting Ethereum amounts to their equivalent USD value.

- `getPrice()`: Retrieves the current price of Ethereum in USD from the Chainlink Oracle.
- `getConversionRate(uint256 ethAmount)`: Converts a given amount of Ethereum to its equivalent value in USD.

## FundMe Contract

The FundMe contract allows users to contribute funds and ensures that the contributed amount meets a minimum threshold in USD value.

### Features:

- **Minimum Contribution**: Users must contribute a minimum amount of USD equivalent in Ethereum to participate.
- **Contribution Tracking**: Tracks the amount contributed by each address and maintains a list of funders.
- **Withdrawal**: Allows the owner of the contract to withdraw the accumulated funds.

## Usage

To use the FundMe smart contract:

1. Deploy the contract to the Ethereum blockchain.
2. Users can contribute funds by calling the `fund()` function and sending Ethereum to the contract.
3. The contract owner can withdraw the accumulated funds by calling the `withdraw()` function.

## Contributing

Contributions to this repository are welcome! If you have any suggestions, improvements, or bug fixes, feel free to open an issue or submit a pull request.

## License

This repository is licensed under the MIT License.
