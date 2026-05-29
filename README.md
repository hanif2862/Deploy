# IOPN Network Smart Contract Deployment

This repository contains a simple Solidity smart contract deployed as part of the IOPN Network on-chain activity. The project demonstrates basic smart contract development, deployment, ownership management, and blockchain interaction on an EVM-compatible network.

The contract allows a user to initialize a name during deployment, update the stored name through an owner-restricted function, and retrieve a greeting message generated from the current stored value. Additionally, every name update is recorded on-chain through an emitted event, providing transparency and traceability of state changes.

The project was developed using Solidity version 0.8.22 and deployed through Remix IDE with a Web3 wallet connection. It serves as a practical example of interacting with blockchain smart contracts and verifying deployment activity within the IOPN Network ecosystem.

## Smart Contract Features

- Smart contract deployment on-chain
- Ownership-based access control
- Public state variable storage
- Event emission for state updates
- Read-only blockchain interaction functions
- EVM-compatible implementation

## Deployment Workflow

The contract was compiled using Solidity Compiler version 0.8.22 in Remix IDE and deployed through a connected wallet. During deployment, an initial name parameter is provided and stored permanently on-chain. After deployment, the contract owner can update the stored name while other users can interact with the public read functions.

## Main Functions

### `changeName(string _newName)`

Allows the contract owner to update the stored name.

### `greet()`

Returns a greeting message generated from the current stored name.

Example output:

```text
Hello, IOPN!
```

### `name()`

Returns the currently stored name.

### `owner()`

Returns the wallet address of the contract owner.

## Purpose

This project was created to demonstrate:

- Smart contract development using Solidity
- Successful on-chain deployment
- Ownership and permission management
- Event logging and blockchain transparency
- Participation in the IOPN Network ecosystem

## Security

The contract implements an ownership model using an `onlyOwner` modifier, ensuring that only the contract owner can execute sensitive state-changing functions. All transactions and updates are permanently recorded on-chain and can be independently verified through a blockchain explorer.

## Technologies Used

- Solidity ^0.8.22
- Remix IDE
- MetaMask Wallet
- EVM-Compatible Blockchain
- IOPN Network Ecosystem

## License

MIT License
