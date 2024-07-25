# Jep Token Smart Contract

## Overview

The ```Jep``` smart contract is an ERC20 token implementation using Solidity. This contract extends the OpenZeppelin ERC20 and Ownable contracts to provide basic token functionality with additional minting and burning capabilities.

## Features

  * ERC20 Token Standard: Implements standard functions and events for an ERC20 token.
  * Minting: Allows the contract owner to mint new tokens.
  * Burning: Allows users to burn (destroy) their own tokens.
  * Custom Transfer: Overrides the default transfer function, though in this case it simply calls the inherited method.

## Installation

1. Install dependencies using hardhat
   
  ```npm install @openzeppelin/contracts```

## Usage

1. Minting Tokens
   
   ```function mint(address to, uint256 amount) public onlyOwner;```

3. Burning Tokens
   
   ```function burn(uint256 amount) public;```

5. Transferring Tokens
   
   ```function transfer(address recipient, uint256 amount) public override returns (bool);```

   
