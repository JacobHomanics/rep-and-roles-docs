1. Clone this repo & install dependencies

```
git clone https://github.com/atxdao/reputation-and-roles-monorepo.git
cd reputation-and-roles-monorepo
yarn install
```

2. In your terminal, clone the environemnt example

```
cd packages/foundry
cp .env.example .env
```

3. On the first terminal, run a local network:

```
yarn chain
```

4. On the second terminal, start your NextJS app:

```
yarn start
```

Visit your app on: `http://localhost:3000`.

Connect a burner wallet.

Copy the wallet address.

Return to your code editor, navigate to `~/packages/foundry/script/Deploy.s.sol`, and replace the value of the `controller` variable with your copied wallet address (make sure to save your file after doing so!).

This command starts a local Ethereum network using Foundry. The network runs on your local machine and can be used for testing and development.

5. On a third terminal, deploy the test contract:

```
yarn deploy
```

This command deploys a test smart contract to the local network. The contract is located at `packages/foundry/lib/reputation/src/ReputationTokensStandalone.sol`.

The `yarn deploy` command uses the deploy script located in `packages/foundry/script/Deploy.s.sol` to deploy the contract to the network. You can also customize the deploy script.

6. View results on webpage

Re-visit your app on: `http://localhost:3000`.

Refresh the page if you need to!

On the home page, you should see many colorful and variable cards and widgets which display your Reputation Tokens in full force!

By navigating to the `Debug Contracts` page, you can interact with and view the properties of your deployed Reputation System!
