# MyToken Solidity Contract

This Solidity contract implements a simple token (coin) with functionality to mint and burn tokens.

## Requirements

1. The contract stores details about the token: Token Name, Token Abbreviation, and Total Supply.
2. It maintains a mapping of addresses to token balances.
3. It has a mint function to increase the total supply and the balance of a specific address.
4. It has a burn function to decrease the total supply and the balance of a specific address, with conditions to ensure the balance is sufficient for burning.

## Usage

### Deployment

1. Compile the `MyToken.sol` contract using a Solidity compiler (version 0.8.7 or higher).
2. Deploy the compiled contract to the Ethereum blockchain.

### Interacting with the Contract

#### Mint Tokens

Use the `mint` function to create new tokens:

```solidity
function mint(uint amount, address recipient) public {
    // Functionality to mint 'amount' tokens for 'recipient'
}
```
#### Burn Tokens
Use the 'Burn' function to burn amount from tokens:
```solidity
function burn(uint amount, address owner) public returns (string memory) {
    // Functionality to burn 'amount' tokens owned by 'owner'
}
```

#### Example
```solidity
// Instantiate the MyToken contract
MyToken myToken = new MyToken();

// Mint 100 tokens to a specific address
myToken.mint(100, 0x123...);

// Burn 50 tokens from the same address
myToken.burn(50, 0x123...);
```

## License
This contract is licensed under the MIT License.
