# Blockchain Smart Ballot - Secure Blockchain Balloting

**Blockchain Smart Ballot** is a decentralized voting system implemented using Solidity. The smart contract allows deployment on a blockchain, enabling users to cast votes with real-time updates. Each user is restricted to vote only once to ensure fairness.
  
## Features
* Blockchain Deployment: Deploy the voting smart contract to a blockchain using Truffle.
* One-Person-One-Vote: Ensures that a single user can vote only once.
* Instant Updates: Reflects voting results in real-time.

## Usage
### Casting a Vote:
* Follow the prompts in the interaction script to vote.
* Each account can only vote once.

### Checking Results:
* Results are updated instantly after each vote.
* Use the interaction script to query the current results.

## Prerequisites
To run this project, ensure you have the following installed:

* Node.js (v16 or higher)
* NPM or Yarn
* Truffle (v5 or higher)
* Ganache (for local blockchain testing)

## Installation
### 1. Clone the Repository:
```bash
git clone https://github.com/bhavinmultiqos/blockchain-smart-ballot.git
cd blockchain-smart-ballot
```
### 2. Install Dependencies:
```bash
npm install
```
### 3. Install Truffle (if not already installed):
```bash
npm install -g truffle
```
### 4. Install Ganache (if not already installed):
```bash
npm install -g ganache-cli
```
### 5. Start Ganache
```bash
ganache-cli --deterministic --port 8545
```
* --deterministic ensures that the same set of accounts is generated each time.
* --port 8545 specifies the port (you can change it if necessary).
Once you run these commands, Ganache will start up and provide an RPC endpoint that you can use in your Truffle configuration, typically http://127.0.0.1:8545.

### 6. Connect MetaMask to the local Ganache blockchain:
1. Open MetaMask and select the network dropdown at the top.
2. Choose "Custom RPC".
3. Enter the following details:
    - Network Name
    - New RPC URL
    - Chain ID
4. Save and switch to the local network.

## Smart Contract Deployment
### 1. Compile the Smart Contract:
```bash
truffle compile
```
### 2. Migrate the Smart Contract:
Update the migrations/2_deploy_contracts.js file with your smart contract deployment logic.

Deploy the smart contract:
```bash
truffle migrate
```

## Interact with the Smart Contract: 
Use the interaction script (test-scripts/interact.js) to interact with the contract after deployment.
Provides functionality to:

* Cast a vote.
* Check the results.
To run the interaction script:
```bash
truffle exec test-scripts/interact.js
```
## Development:
### 1. Testing: 
Write tests for the smart contract in the test/ directory and run:
```bash
truffle test
```
### 2. Modify the Contract:
The smart contract source code is in contracts/Voting.sol. Make necessary changes and recompile/migrate as needed.

## Contributing
Contributions are welcome! Please create an issue or pull request for any suggestions or improvements.

## License
This project is licensed under the MIT License.

## Let Us know
For more details, visit [MultiQoS](https://multiqos.com/).


