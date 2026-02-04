# Governor DAO Core

This repository provides a modular and secure framework for decentralized governance. It follows the **Governor** standard, which is the most widely adopted architecture for DAOs (used by Uniswap, Compound, and Aave).



## Components
* **Governance Token**: An ERC20 token with snapshotting capabilities for voting power.
* **Timelock Controller**: Adds a mandatory delay between a proposal passing and its execution, allowing users to exit if they disagree.
* **Governor Contract**: The logic engine that handles quorum, voting periods, and proposal thresholds.

## Governance Process
1. **Proposal**: A token holder with enough voting power submits a proposal.
2. **Voting**: Holders cast votes (For, Against, or Abstain) during the voting window.
3. **Queueing**: If passed, the proposal enters the Timelock.
4. **Execution**: After the delay, the proposal is executed on-chain.

## License
MIT
