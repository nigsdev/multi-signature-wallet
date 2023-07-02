## 👛 Multisig Wallet


### 🏃‍♀️ Quick Start

required: [Node](https://nodejs.org/dist/latest-v12.x/) plus [Yarn](https://classic.yarnpkg.com/en/docs/install/) and [Git](https://git-scm.com/downloads)

```bash

yarn install

```

```bash

yarn start

```

> in a second terminal window:

```bash
yarn chain

```

📱 Open http://localhost:3000 to see the app

> in a third terminal window:

```bash
yarn backend

```

🔧 Configure your deployment in `packages/hardhat-ts/deploy/01_deploy_meta_multi_sig_wallet_contract.ts`

> Edit the chainid, your owner addresses, and the number of signatures required:


> in a fourth terminal deploy with your frontend address as one of the owners:

```bash

yarn deploy

```


> Use the faucet wallet to send your multi-sig contract some funds:

![image](https://user-images.githubusercontent.com/31567169/118389510-53315600-b63b-11eb-9daf-f0aaa479a23e.png)

> To add new owners, use the "Owners" tab:


![image](https://user-images.githubusercontent.com/31567169/118389556-896ed580-b63b-11eb-8ed6-c1e690778c8e.png)

This will take you to a populated transaction create page:

![image](https://user-images.githubusercontent.com/31567169/118389576-9986b500-b63b-11eb-8411-c227b148992a.png)




> Create & sign the new transaction:

![image](https://user-images.githubusercontent.com/31567169/118389603-ae634880-b63b-11eb-968f-ca78c2456ddb.png)


You will see the new transaction in the pool (this is all off-chain):

![image](https://user-images.githubusercontent.com/31567169/118389616-bd49fb00-b63b-11eb-82f7-f65ca2ee7e80.png)


Click on the ellipsses button [...] to read the details of the transaction


![image](https://user-images.githubusercontent.com/31567169/118389642-d6eb4280-b63b-11eb-9676-da7e7afc5614.png)



> Give your account some gas at the faucet and execute the transaction

The transction will appear as "executed" on the front page:

![image](https://user-images.githubusercontent.com/31567169/118389655-e8cce580-b63b-11eb-8428-913c6f39e48f.png)



> Create a transaction to send some funds to your frontend account:

![image](https://user-images.githubusercontent.com/31567169/118389693-0ef28580-b63c-11eb-95d9-c5f397bf5972.png)




This time we will need a second signature:

![image](https://user-images.githubusercontent.com/31567169/118389716-3cd7ca00-b63c-11eb-959e-d46ffe31e62e.png)



> Sign the transacton with enough owners:
![image](https://user-images.githubusercontent.com/31567169/118389773-90e2ae80-b63c-11eb-9658-e9c411542f33.png)


(You'll notice you don't need ⛽️gas to sign transactions.)

> Execute the transction to transfer the funds:



![image](https://user-images.githubusercontent.com/31567169/118389808-bff92000-b63c-11eb-9107-9af5b77d4e20.png)