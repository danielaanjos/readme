<h1 align="center">TITLE</h1>

Description

## :computer: System requirements

[![NPM](https://img.shields.io/badge/NPM-%23000000.svg?style=for-the-badge&logo=npm&logoColor=white)](https://www.npmjs.com/)
[![Angula CLI](https://img.shields.io/badge/angular-%23DD0031.svg?style=for-the-badge&logo=angular&logoColor=white)](https://www.npmjs.com/package/@angular/cli)


## :rocket: How to install

 Access the directory of the project and run the command below.

``` sh
$ npm install
```

## :coffee: How to create the environment

1. Access the ```src/environment```directory of the project

2. Create an .env file within the project following the example:

``` sh
export const environment = {
  production: If you are in a development and approval environment, choose false, if it is true production.,
  scryptDiff: 14,
  API_COUNTRY: 'https://restcountries.eu/rest/v2/all',
  blockchainNode: 'https://ropsten.infura.io/v3/60b04b44120540eba51cd97de49b479b',
  ccoinTokenAddress: '0x8B0bcf086e00CDAE3417CfdD49322Ec44C1d56E2',
  daiTokenAddress: '0xE7D698fB1700e3a8eFE68E4fC13579796AE51B99',
  swapContractAddress: '0x32eF558E2a59c9C44C67320dce4a5077aDaFBC44',
  ethGasStationKey: 'c8ba7be38fcab6f755c62033e827d385e8fcbea67de6a5277a39ef4f88a8',
  whitelistContractAddress: '0x1322bbc012B5De09D6D79427A52951ff015b18E7',
  PayloadKey: 'Generate random key that will be used for payload encryption, the same generated key needs to be in the envs of the APIs that have the example',
  SaltKey: 'Executes simple management of Salt server public keys used for authentication',
  Apis: {
    accessControl: 'API address and port',
    deposit: 'API address and port',
    kyc: 'API address and port',
    storage: 'API address and port',
    message: 'API address and port',
    core: 'API address and port',
    rebuy: 'API address and port',
    offers: 'API address and port',
  },
  providerOptions: {
    useCustomRpc: false,
    customRpcURL: 'http://localhost:8545',
    network: 'ropsten',
    alchemy: '',
    etherscan: '',
    infuraId: '',
    infuraSecret: '',
  },
};
```

| Definition | Description |
| ---------- | ----------- |
| **production** | If you are in a development and approval environment, choose false, if it is true production. |
| **scryptDiff** | Degree of difficulty in creating the user's wallet, as the wait in wallet generation increases, it is greater but safer. |
| **API_COUNTRY** | Global API to load countries listed on the platform |
| **blockchainNode** | blockchain network URL address |
| **ccoinTokenAddress** | Contract number that was deployed on the blockchain network |
| **daiTokenAddress** | Contract number that was deployed on the blockchain network |
| **swapContractAddress** | Contract number that was deployed on the blockchain network |
| **ethGasStationKey** | Key created in etherscan for Ethereum network |
| **whitelistContractAddress** | Contract number that was deployed on the blockchain network |
| **PayloadKey** | Generate random key that will be used for payload encryption, the same generated key needs to be in the envs of the APIs that have the example |
| **SaltKey** | Executes simple management of Salt server public keys used for authentication. |
| **Apis** | List of apis to connect services app.|
| **providerOptions** | Service dependencies. |

- Provider Options parameters:

| Definition | Description |
| ---------- | ----------- |
| **useCustomRpc** | If you want to configure a custom rpc server choose true, if not false. |
| **customRpcURL** | If you chose true in useCustomRPC, enter the link URL |
| **network** | blockchain network name|
| **alchemy** |Key created in alchemy for Ethereum network |
| **etherscan** | Key created in etherscan for Ethereum network |
| **infuraId** | Key created in Infura for Ethereum network |
| **infuraSecret** | Key password created in Infura for Ethereum network |
## Run server

Access the directory of the project and run one of the commands below.

- **development:**
``` sh
$ npm run start
```

- **QA:**
``` sh
$ npm run start:qa
```

Navigate to ```http://localhost:4200/```.
The app will automatically reload if you change any of the source files.

##  :hammer: Build

Access the directory of the project and run the command below.

- **build**
``` sh
$ npm run build
```

The build artifacts will be stored in the ```dist/ ```directory. Use the ```--prod``` flag for a production build.

## Tests
Access the directory of the project and run one of the commands below.

- **unit tests** 
Run command to execute the unit tests via [Karma](https://karma-runner.github.io/).
``` sh
$ npm run test
```

- **e2e tests**
Run command to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).
``` sh
$ npm run e2e
```
