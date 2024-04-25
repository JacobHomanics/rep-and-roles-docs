# Roles
There are several roles (unrelated to the Roles portion of this project) which have different responsibilities for managing and operating a specific instance of a Reputation system. 

## Admin
An Admin has the ability to grant/revoke any other roles from another address, including itself.

## Minter
A Minter has the ability to mint new tokens to any address. By doing so, this will update the balance of the recipient address and also flag those tokens for only distribution.
## Token Migrator

The token migrator acts as a utility role serving the purpose migrating existing Reputation token (regardless of token type constraints) from one account to another.

This is useful for the case where a DAO member's wallet gets compromised and they need to have a way to transfer their existing tokens to their new address. This prevents unnecesary tokens from being minted.

## Psuedo-Roles

There are severral psuedo roles present in the smart contract. This means that they are not an explicit role defined by the smart contract, however, based on circumstances, an address could be considered as having the specific psuedo-role.

### Distributor
A Distributor is an address who has been minted a number of tokens. Those tokens are flagged for distribution and cannot be transferred through regular means.
### Burner
A Burner is an address who has received Redeemable tokens from another address.