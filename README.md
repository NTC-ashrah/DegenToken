# DegenToken

DegenToken is an ERC20 token with additional functionalities such as minting, burning, and an in-game store for redeeming tokens for special items. This smart contract is built using Solidity and leverages the OpenZeppelin library for secure and standard token implementation.

Features
Minting: Only the contract owner can mint new tokens.
Burning: Token holders can burn their own tokens.
Transfer: Token holders can transfer tokens to other addresses.
Store Items: Token holders can redeem their tokens for in-game items.
Contract Details
Name: Degen
Symbol: DGN
Decimals: 0
Functions
mint(address to, uint256 amount)
Mints new tokens to the specified address. Only the owner can call this function.

Parameters:

to: Address to mint tokens to.
amount: Number of tokens to mint.
decimals()
Returns the number of decimal places the token uses. This contract uses 0 decimals.

getBalance()
Returns the token balance of the caller.

transferTokens(address _receiver, uint256 _value)
Transfers tokens from the caller to the specified receiver.

Parameters:

_receiver: Address to transfer tokens to.
_value: Number of tokens to transfer.
burnTokens(uint256 _value)
Burns the specified number of tokens from the caller's balance.

Parameters:

_value: Number of tokens to burn.
showStoreItems()
Displays the items available for in-game purchase.

redeemTokens(uint8 _userChoice)
Redeems tokens for in-game items based on the user's choice.

Parameters:

_userChoice: Selection of the item to redeem (1 for Wings, 2 for Costume, 3 for Lucky Box).
Player Items
Each player can have the following items:

Wings: Limited Edition Degen Wings
Costume: Lord Degen Costume
Lucky Box: Degen Lucky Box
Usage
Deployment
Deploy the contract to the Ethereum blockchain using a tool like Hardhat or Truffle. Make sure to have the required dependencies installed, including OpenZeppelin contracts.

Interacting with the Contract
Mint Tokens: The owner can mint new tokens to any address.
Transfer Tokens: Token holders can transfer tokens to others.
Burn Tokens: Token holders can burn their own tokens to decrease supply.
Redeem Items: Token holders can redeem their tokens for special in-game items.
Example
To mint 1000 Degen tokens to an address:

solidity
Copy code
degenToken.mint("0xAddress", 1000);
To redeem a Degen Lucky Box:

solidity
Copy code
degenToken.redeemTokens(3);
License
This project is licensed under the MIT License. See the LICENSE file for details.



