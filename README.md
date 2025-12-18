MyToken (MTK) — ERC-20 Token Project
📌 Overview

MyToken (MTK) is an ERC-20 compliant fungible token written in Solidity and deployed using Remix IDE.
This project demonstrates the fundamental concepts behind ERC-20 tokens on the Ethereum blockchain, including token transfers, allowances, delegated transfers, and event emissions.

The project is intended for learning and demonstration purposes.

🔗 Token Details
Property	Value
Name	MyToken
Symbol	MTK
Decimals	18
Total Supply	1,000,000 MTK
Initial Mint	Entire supply minted to deployer
On-chain totalSupply Value

Due to 18 decimals:

1000000000000000000000000

What is an ERC-20 Token?

ERC-20 is the official Ethereum standard for fungible (interchangeable) tokens.
It defines a common interface that ensures compatibility with:

Wallets

Exchanges

Decentralized applications (dApps)

Other smart contracts

Core ERC-20 Behaviors

Transfer tokens between addresses

Track account balances

Approve another address to spend tokens

Perform delegated transfers using transferFrom

Emit Transfer and Approval events

✨ Implemented Features
✔ Balance Tracking

balanceOf(address) — returns token balance

✔ Direct Transfers

transfer(address to, uint256 amount)

Moves tokens from sender to recipient

✔ Allowance System

approve(address spender, uint256 amount) — grants spending permission

allowance(address owner, address spender) — checks approved amount

✔ Delegated Transfers

transferFrom(address from, address to, uint256 amount)

Spends tokens using approved allowance

✔ Events

Transfer — emitted on token movement

Approval — emitted when allowance is set

✔ Validations

Prevent transfers to zero address

Ensure sufficient balance

Ensure sufficient allowance

🚀 Deployment Instructions (Remix IDE)
1️⃣ Open Remix

Visit: https://remix.ethereum.org/

2️⃣ Add Contract

Create the file:

/contracts/MyToken.sol


Paste the Solidity contract code.

3️⃣ Compile

Compiler version: Solidity 0.8.x

Click Compile MyToken.sol

4️⃣ Deploy

Environment: Remix VM (Prague)

Initial supply:

1000000000000000000000000


Click Deploy

📝 Usage Examples
🔹 Check Balance
balanceOf(0xYourAddress)

🔹 Transfer 1 MTK
transfer(0xRecipient, 1000000000000000000)

🔹 Approve 5 MTK
approve(0xSpender, 5000000000000000000)

🔹 Delegated Transfer (2 MTK)
transferFrom(
  0xOwner,
  0xReceiver,
  2000000000000000000
)

🧪 Testing Performed
✔ Metadata Verification

Name

Symbol

Decimals

Total Supply

✔ Transfer Test

Sent 1 MTK from Account A → B

✔ Approval Test

Approved Account B to spend 5 MTK

✔ transferFrom Test

Account B transferred 2 MTK from A → C

✔ Edge Case Handling

Zero-address transfer → reverted

Insufficient balance → reverted

Insufficient allowance → reverted

📸 Screenshots

Screenshots are stored in the /screenshots directory:

compilation.png

deployment.png

token-info.png

transfer-test.png

events.png

📚 What I Learned

Internal working of ERC-20 tokens

Allowance and delegated transfer mechanism

Importance of blockchain events for transparency

Contract compilation, deployment, and testing using Remix

Best practices like validations and event logging

📂 Project Structure
my-token/
├── contracts/
│   └── MyToken.sol
├── screenshots/
│   ├── compilation.png
│   ├── deployment.png
│   ├── token-info.png
│   ├── transfer-test.png
│   └── events.png
└── README.md

✅ Submission Ready

This project includes:

✔ Fully working ERC-20 token

✔ Required screenshots

✔ Complete documentation

✔ Successful functional testing

✔ Clean and readable Solidity code