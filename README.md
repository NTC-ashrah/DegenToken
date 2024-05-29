# DegenToken
Project: Degen Token (ERC-20): Unlocking the Future of Gaming (Module 4)

DegenToken
DegenToken is an ERC20 token with capabilities for minting, burning, transferring, and redeeming tokens for in-game items.

Features
Minting: Contract owner can mint new tokens.
Burning: Token holders can burn their tokens.
Token Transfer: Tokens can be transferred between holders.
In-Game Store: Tokens can be redeemed for in-game items.
Token Details
Name: Degen
Symbol: DGN
Decimals: 0
Installation
Clone the repository:

git clone <repository_url>
cd <repository_directory>
Install dependencies:

npm install
Compile the contract:

npx hardhat compile
Usage
Deploying the Contract
Deploy to a local network:
npx hardhat node
npx hardhat run scripts/deploy.js --network localhost
Interacting with the Contract
Mint Tokens: Function to mint new tokens
function mint(address to, uint256 amount) public onlyOwner
Burn Tokens: Function to burn tokens
function burnTokens(uint256 _value) external
Get Balance: Function to get the balance of tokens
function getBalance() external view returns (uint256)
Transfer Tokens: Function to transfer tokens to another address
function transferTokens(address _receiver, uint256 _value) external
Show Store Items: Function to display available in-game store items
function showStoreItems() external pure returns (string memory)
Redeem Tokens for Store Items: Function to redeem tokens for in-game store items
function redeemTokens(uint8 _userChoice) external payable returns (bool)
License
This project is licensed under the MIT License.






