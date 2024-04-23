# Roles
There are several roles (unrelated to the Roles portion of this project) which have different responsibilities for managing and operating a specific instance of a Reputation system. 

## Minter

Can mint Reputation tokens ONLY TO Distributors.

The minter is typically granted to a multi-sig or ledger. The minter controls the outflowing supply of tokens into the ecosystem. Thus, it should only be granted
to trusted and safeguarded addresses. The minter and distributor role needs to be split, for in the case of the distributor role getting compromised, it can become flagged and never receive
tokens to distribute ever again. If a minter becomes compromised then you can assume the system is jacked and unrecoverable. Thus for the need for minters to be safeguarded very securely and only minting tokens to distributors on an as needed basis.

## Distributor

Minter mints tokens to distributor. 

Can distribute minted Reputation tokens to ANY entity.

## Entity
Entity is virtually every address on the blockchain. 
A role does not exist on the smart contract level for an entity.
An entity is an address that can transfer tokens based on their token types and not through the regulations imposed by Minter, Distributor, Burner, or Token Migrator roles.

## Burner

Can receive Redeemable tokens from another address. Received tokens through burning can never be transfered again. They are effectively burned. These are most effective as a smart contract which initiates the burn transaction for the entity and runs arbitrary code either before or after the transfer, but can optionally be a regular EOA where offchain rewards are awarded.

## Token Migrator

The token migrator acts as a utility role serving the purpose migrating existing Reputation token (regardless of token type constraints) from one account to another.

This is useful for the case where a DAO member's wallet gets compromised and they need to have a way to transfer their existing tokens to their new address. This prevents unnecesary tokens from being minted.