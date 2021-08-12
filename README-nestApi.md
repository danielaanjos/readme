<h1 align="center">TITLE</h1>

Description

## :computer: System requirements

[![NodeJS](https://img.shields.io/badge/node.js-%2343853D.svg?style=for-the-badge&logo=node.js&logoColor=white)]((https://nodejs.org/en//))
[![NPM](https://img.shields.io/badge/NPM-%23000000.svg?style=for-the-badge&logo=npm&logoColor=white)](https://www.npmjs.com/)
[![NestJS](https://img.shields.io/badge/nestjs-%23E0234E.svg?style=for-the-badge&logo=nestjs&logoColor=white)](https://nestjs.com/)
[![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)](https://docs.docker.com/compose/install/#install-compose)

## :rocket: How to install

 Access the directory of the project and run the command below.

``` sh
$ npm install
```

## :coffee: How to create the environment

1. Access the directory of the project and run the command below.

``` sh
$ docker-compose up -d
```

This command will creates and execute the containers defined in the docker-compose.yml file.

2. Create an .env file within the project following the example:

``` sh
PORT=3004
NOSQL_CONNECTION_STRING='mongodb://4cadia:Passw0rd@127.0.0.1:27022/poperp-financeiro'
SALT_KEY='string'
JWT_KEY='string'
JWT_EXPIRATION=3600
```

| Definition | Description |
| ---------- | ----------- |
| **PORT** | Virtual point where network connections |
| **NOSQL_CONNECTION_STRING** | String used to access a database |
| **SALT_KEY** | Executes simple management of Salt server public keys used for authentication. |
| **JWT_KEY** | Symmetric key that is known by both the sender and the receiver.|
| **JWT_EXPIRATION** | Expiration time on or after which the JWT MUST NOT be accepted for processing. |

## Running the API

Access the project directory and run one of the commands below.

- **Development:**
``` sh
$ npm run start
```
- **Assisted mode development**
``` sh
$ npm run start:dev
```
- **Production**
``` sh
$ npm run start:prod
```

## :page_with_curl: Documentation

After running the api access the local host

Example: http://localhost:3000