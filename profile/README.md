# Welcome to Terragrids
## TL;DR
[Terragrids](https://terragrids.org) is a web3 crowd-funding platform for community renewable energy projects. 

The online crowdfunding platform is a game built on top of the Algorand blockchain. It runs a small metaverse, where participants can explore, build and develop a sustainable town entirely powered by renewable energy. 

Players buy and own NFTs to develop the Terragrids world on the virtual map. The revenues from the purchase of each NFT will be administered in the Terragrids treasury Algorand wallet and will directly contribute to the planning and delivery of real community renewable energy projects across the globe.

NFTs will give players governance rights in the management of the Terragrids metaverse, gradually developing Terragrids into a DAO.

## Tech stack
Terragrids Algorand smart-contracts are developed using [Reach](https://www.reach.sh). 

The front-end is a React application, with a node.js backend. 

NFTs are [ARC3](https://github.com/algorandfoundation/ARCs/blob/main/ARCs/arc-0003.md) with media files pinned on [Pinata IPFS](https://www.pinata.cloud/).

All repositories are open-sourced on GitHub.

## Get Started
To get started and contribute to the development, you will need to clone the following repositories:
* `api` - the node.js API to interface with the DynamoDB off-chain storage and the Algo indexer API
* `db-scripts` - a collection of useful development scripts for your local dynamodb instance
* `dapp` - the front-end for the Algorand distributed application and the Reach program to deploy and run smart contracts
* `project-contract` - the node.js API and the Reach program to deploy and access smart contracts handling project crowdfunding

After cloning these repositories, head to the `README` and follow the setup instruction for each one.

## Contributions

To make contributions, check out the `dev` branch in the repo you want to make a code change, create a personal branch, name it starting with `feature/`, and push your commits. When you are ready, open a Pull Request on the `dev` branch.

**Dev rules**

1. Please use Visual Code with `Prettier` extension installed to write changes and make contributions to the repository. This will ensure code standard consistency.
2. Make small Pull Requests. This will ensure other developers and project maintainers can review your changes and give feedback as quickly as possible.
3. Never make a Pull Request on `master`. The `master` branch is regularly updated with `dev` only by project maintainers.
