# Roles

Roles utilizes Reputation to grant authorities and responsibilities through the use of the Hats Protocol.

Hats make use of their own ERC1155 tokens which are used to assign roles through Onchain/Offchain means. 

The Hats protocol consists of a single tree (The Hats Protocol). Within this tree, are a bunch of branches (organizations, entities, companies), and within those branches are a bunch of leaves (Hat ERC1155 Token). Each leaf (or Hat) contains its own responsibilities, usually within the context of its branch (i.e. organization). Entities can come along and hold (wear) a leaf to be granted a certain role, again within the context of the organization. 

The Reputatuion & Roles project utilizes the Hats Protocol by each Reputation project having its own branch. Hats are special, because they have something called Eligibility Modules. One module, of particular interest within R&R is the ERC1155 Eligibility Module. This module only allows for users to Claim and continuously Wear Hats only if they maintain a certain threshold of ERC1155 tokens. And what are Reputation Tokens? That's right, ERC1155 Tokens! This means we can properly gate roles behind Hats by using their ERC1155 Eligiblity Module in connjunction with Reputation Tokens! Wonderful.

The Reputation & Roles Monorepo project contains a copy of the Hats smart contracts that are present on Testnet/Mainnet. Thus, when we deploy locally we also created a Faux Hats Protocol. Simply for ease of use and improved development flows. However, once your Reputation & Roles project graduates to Testnet/Mainnet, then your project should automatically point to the proper smart contract addresses and implementations.

For more info on Hats, then please go to their [Website](https://www.hatsprotocol.xyz/) or visit their [docs](https://docs.hatsprotocol.xyz/) to gain a deeper understanding.


